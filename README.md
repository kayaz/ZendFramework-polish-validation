# ZendFramework-polish-validation
Using in forms:

    // Polskie tlumaczenie errorów
    $polish = kCMS_Polish::getPolishTranslation();
    $translate = new Zend_Translate('array', $polish, 'pl');
    $this->setTranslator($translate);

Using in controllers:

    $form = new Form_BasicForm();
    $this->view->form = $form;

    // Polskie tlumaczenie errorów
    $polish = kCMS_Polish::getPolishTranslation();
    $translate = new Zend_Translate('array', $polish, 'pl');
    $form->setTranslator($translate)
