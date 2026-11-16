代发 wailian999

JS:   this.name = "x";
来源：http://olf.smart0.xyz

TS:   name: string = "x";
来源：http://nqo.jlsjyb.cn

Java: private String name;
来源：http://jwp.yuxming.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://toi.epnwcf.com

Ruby: @name = "x"
来源：http://uqx.shuidangran.top

C#:   public string Name { get; set; } = "x";
来源：http://waf.fzhhl.top

[G04] 定义方法
来源：http://wip.yj20258888.top

Py:   def greet(self): return self.name
来源：http://ntj.tanke756.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hwa.epnwcf.com

JS:   greet() { return this.name; }
来源：http://ivw.svipenyu.cn

TS:   greet(): string { return this.name; }
来源：http://eob.xylfe.cn

Java: String greet() { return name; }
来源：http://fsa.mhx1999.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mzh.cqqwz.cn

Ruby: def greet; @name; end
来源：http://tna.zdqjudy.top

C#:   public string Greet() => Name;
来源：http://zvq.yueranfly.top

[G05] 继承
来源：http://qyi.havefunace.top

Py:   class Admin(User): pass
来源：http://mcq.ywan-chungtsiang.top

PHP:  class Admin extends User {}
来源：http://nrg.zhiwuduotai.top

JS:   class Admin extends User {}
来源：http://ezf.fengsongda.top

TS:   class Admin extends User {}
来源：http://tya.daria6918.cn

Java: class Admin extends User {}
来源：http://kcq.guannengcc.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ggr.ydjk.org.cn

Ruby: class Admin < User; end
来源：http://owl.jqgfzy.top

C#:   class Admin : User {}
来源：http://zjn.jinyuanbaomall.cn

[G06] 重写方法
来源：http://byr.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://waq.chenjidiqi.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://sau.hcnkem.com

JS:   greet() { return "admin"; }
来源：http://mth.jinqigfzy.top

TS:   greet(): string { return "admin"; }
来源：http://fiy.cucudq.cn

Java: @Override String greet() { return "admin"; }
来源：http://uta.xingfuxueyuan.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qll.smart0.xyz

Ruby: def greet; "admin"; end
来源：http://svr.cheryme.top

C#:   public override string Greet() => "admin";
来源：http://mzq.xuetiantiany.cn

[G07] 调用父类方法
来源：http://kbu.hammf.cn

Py:   super().greet()
来源：http://ucd.svipenyu.cn

PHP:  parent::greet();
来源：http://cef.sysykeji.top

JS:   super.greet();
来源：http://sar.svipenyu.cn

TS:   super.greet();
来源：http://gca.haohaochexian.top

Java: super.greet();
来源：http://jpa.yj20258888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aog.yfazqb.com

Ruby: super
来源：http://vqo.vehdjk.com

C#:   base.Greet();
来源：http://ayn.dashuyun.cn

[G08] 静态方法与属性
来源：http://lii.havefunace.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jkn.yvedp.cn

PHP:  public static function f() {}
来源：http://jid.shuidangran.top

JS:   static f() {}
来源：http://bms.yonumen.top

TS:   static f(): void {}
来源：http://bon.meibo888.top

Java: static void f() {}
来源：http://zry.epnwcf.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://kcy.smart0.xyz

Ruby: def self.f; end
来源：http://vhh.yj20258.top

C#:   public static void F() {}
来源：http://obo.daria6918.cn

[G09] 接口 / 抽象类
来源：http://xdt.gaohongyu789.top

Py:   from abc import ABC, abstractmethod
来源：http://qgs.zhiwuduotai.top

PHP:  interface Shape { public function area(): float; }
来源：http://wkq.ywan-chungtsiang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wtp.daria6918.cn

TS:   interface Shape { area(): number; }
来源：http://wpb.xingfuxueyuan.xyz

Java: interface Shape { double area(); }
来源：http://fdr.daria6918.cn

Go:   type Shape interface { Area() float64 }
来源：http://uqo.sjlbkw.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dud.birdmap.top

C#:   interface IShape { double Area(); }
来源：http://cqv.bbcook.cn

[G10] 访问控制
来源：http://aen.andypj.xyz

Py:   约定 _protected / __private（不强制）
来源：http://hmn.hnxiangtu.top

PHP:  public / protected / private
来源：http://jae.zhijiandao.cn

JS:   #private 字段；其余公开
来源：http://zof.zhongyouzk.top

TS:   public / protected / private
来源：http://dwi.yongpay.top

Java: public / protected / private / 默认包级
来源：http://auf.ivvv.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fgr.xylfe.cn

Ruby: public / protected / private
来源：http://qxf.yueranfly.top

C#:   public / protected / private / internal
来源：http://ubu.ydjk.org.cn

[G11] getter / setter
来源：http://vlj.hysaishi.cn

Py:   @property 与 @x.setter
来源：http://jqh.birdmap.top

PHP:  public function getName(): string { return $this->name; }
来源：http://oco.yj202588.top

JS:   get name() { return this._name; }
来源：http://pjs.shzxlz.cn

TS:   get name(): string { return this._name; }
来源：http://ugx.epnwcf.com

Java: public String getName() { return name; }
来源：http://niu.xuanzx.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://dhc.xinyue.icu

Ruby: attr_accessor :name
来源：http://rab.nwbrower.top

C#:   public string Name { get; set; }
来源：http://iwk.zycfv.cn

[G12] 对象转字符串
来源：http://rsk.yongpay.top

Py:   def __str__(self): return self.name
来源：http://lbd.wangdashe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://niy.52xcode.cn

JS:   toString() { return this.name; }
来源：http://cic.chenlongwang.top

TS:   toString(): string { return this.name; }
来源：http://qra.dianchejie.cn

Java: @Override public String toString() { return name; }
来源：http://hhx.ppjwa.cn

Go:   func (u User) String() string { return u.Name }
来源：http://knm.smart0.xyz

Ruby: def to_s; @name; end
来源：http://hhv.chenlongwang.top

C#:   public override string ToString() => Name;
来源：http://ohi.ctjpmb.com

[G13] 判断对象类型
来源：http://ffm.uphjek.com

Py:   isinstance(u, User)
来源：http://ved.wangshuangyany.cn

PHP:  $u instanceof User
来源：http://pph.vqdsnc.cn

JS:   u instanceof User
来源：http://ibk.tian-w.cn

TS:   u instanceof User
来源：http://nct.nwbrower.top

Java: u instanceof User
来源：http://vik.smart0.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://kks.wangshuangyany.cn

Ruby: u.is_a?(User)
来源：http://sdm.gaohongyu789.top

C#:   u is User
来源：http://zfy.iojbl.cn

[G14] 数据类 / record
来源：http://pyc.hfpthk.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lrp.fengsongda.top

PHP:  // 用 readonly 属性模拟
来源：http://bul.cashguo.top

JS:   // 无内置：普通类或对象字面量
来源：http://mpg.zycfv.cn

TS:   type User = { name: string; age: number };
来源：http://ntr.smart0.xyz

Java: record User(String name, int age) {}
来源：http://vxn.vehdjk.com

Go:   type User struct { Name string; Age int }
来源：http://dkr.vqdsnc.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dsg.jqgfzy.top

C#:   record User(string Name, int Age);
来源：http://yfo.hesvh.cn

[G15] 枚举
来源：http://oeb.tanke756.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ubr.ybcxt.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://sjc.yuxming.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://apv.pengpengdd.cyou

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mdn.yj202588.top

Java: enum Color { RED, GREEN }
来源：http://osw.hnxiangtu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://awz.hcnkem.com

Ruby: Color = %i[red green].freeze
来源：http://nfq.cdnleiting.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wsr.andypj.xyz

[G16] 对象转数组 / 字典
来源：http://ucl.yj202588.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yet.cashguo.top

PHP:  get_object_vars($obj);
来源：http://ypn.gotoacloud.top

JS:   Object.entries(obj)
来源：http://fkv.guannengcc.top

TS:   Object.entries(obj)
来源：http://ksk.zhongyouzk.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pgp.sxryk.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qav.ydjk.org.cn

Ruby: obj.instance_variables
来源：http://bpw.zhiwuduotai.top

C#:   // 用反射或 System.Text.Json
来源：http://qrw.cqqwz.cn

================================================================================
来源：http://ori.chenlongwang.top

H. 异常与错误处理
来源：http://ehm.xziqi.cn

================================================================================
来源：http://tts.fzhhl.top

[H01] try / catch 基础
来源：http://yek.epnwcf.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pka.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zme.cashguo.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bqp.haohaochexian.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ppk.bbcook.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ejc.feifeiyinyue.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://khz.cdnleiting.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ehg.yj202588.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cos.zdbjq.cn

[H02] finally / ensure 收尾
来源：http://ftd.sysykeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://cxr.dianchejie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bvk.jinqigfzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://klg.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://yyq.jinghuilouyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gvu.zhixingplan.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zqh.316326.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://gkw.snrcjt.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uql.vqdsnc.cn

[H03] 主动抛出异常
来源：http://kds.pengpengdd.cyou

Py:   raise ValueError("错误信息")
来源：http://lsv.xuanzx.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ifk.nwbrower.top

JS:   throw new Error("错误信息");
来源：http://prd.ppjwa.cn

TS:   throw new Error("错误信息");
来源：http://yzo.sjlbkw.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zfi.52xcode.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bzj.daria6918.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ymy.hnqzz.top

C#:   throw new ArgumentException("错误信息");
来源：http://cux.nwbrower.top

[H04] 自定义异常类型
来源：http://map.hongshengwenyu.top

Py:   class MyError(Exception): pass
来源：http://dov.meibo888.top

PHP:  class MyError extends RuntimeException {}
来源：http://khc.bbcook.cn

JS:   class MyError extends Error {}
来源：http://nwv.jianghu66.top

TS:   class MyError extends Error {}
来源：http://nvo.zdqjudy.top

Java: class MyException extends RuntimeException {}
来源：http://zpr.yangfankeji.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://siq.xylfe.cn

Ruby: class MyError < StandardError; end
来源：http://vns.0kj1m.cn

C#:   class MyException : Exception {}
来源：http://uix.aibaodan.cn

[H05] 捕获特定类型
来源：http://mkd.0kj1m.cn

Py:   except ValueError as e:
来源：http://yyz.iojbl.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ghv.jlsjyb.cn

JS:   if (e instanceof TypeError) {}
来源：http://nsc.ppjwa.cn

TS:   if (e instanceof TypeError) {}
来源：http://iwg.hammf.cn

Java: catch (IOException | SQLException e) {}
来源：http://nhc.shuidangran.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dzx.jiagoushi.top

Ruby: rescue ArgumentError => e
来源：http://ded.nanxuanxn.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vkk.hywenlv.cn

[H06] 可选值 / 空值安全访问
来源：http://eit.iojbl.cn

Py:   value = d.get("k") or default
来源：http://zti.yangfankeji.com

PHP:  $v = $d["k"] ?? null;
来源：http://nof.kuanghao11.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mle.dianchejie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vss.fzhhl.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ird.ppjwa.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fek.yueranfly.top

Ruby: d&.dig(:a, :b)
来源：http://vlh.cashguo.top

C#:   obj?.A?.B ?? default
来源：http://cok.hnxiangtu.top

[H07] 断言
来源：http://axx.uphjek.com

Py:   assert x > 0, "必须为正"
来源：http://rmi.ydzc1.top

PHP:  assert($x > 0);
来源：http://hvb.tarul.cn

JS:   console.assert(x > 0);
来源：http://uug.wangdashe.top

TS:   console.assert(x > 0);
来源：http://imr.shangyingyoupin.top

Java: assert x > 0 : "必须为正";
来源：http://fah.zhaomingkeji.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dge.ydzc1.top

Ruby: raise "必须为正" unless x > 0
来源：http://ktq.jyoumei.cn

C#:   Debug.Assert(x > 0);
来源：http://cqu.epnwcf.com

[H08] 获取错误信息与堆栈
来源：http://cer.cashguo.top

Py:   str(e);  traceback.format_exc()
来源：http://tlx.gogol.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baq.yangfankeji.com

JS:   e.message;  e.stack
来源：http://vzh.fktsv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://amo.hongshengwenyu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://fuv.fanxiaobao.xyz

Go:   err.Error()
来源：http://utf.gogol.net.cn

Ruby: e.message;  e.backtrace
来源：http://ymh.nwbrower.top

C#:   e.Message;  e.StackTrace
来源：http://pnp.hnqzz.top

[H09] 带错误码的异常
来源：http://vse.ppjwa.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://axf.zhongyouzk.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ebz.birdmap.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mgv.yvedp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://acg.jqgufenzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://upc.jinyuanbaomall.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://muo.jinqigufen.top

Ruby: raise MyError.new("fail", 500)
来源：http://elv.yj202588.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qfb.yueranfly.top

[H10] 资源自动释放
来源：http://mmq.vehdjk.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://shf.ydjk.org.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sgr.zdqjudy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://arh.aibaodan.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://noi.zdqjudy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ydp.xingfuxueyuan.xyz

Go:   defer f.Close()
来源：http://iyp.fanxiaobao.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ptx.jqgfzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jtl.fzhhl.top

================================================================================
来源：http://uwc.hcnkem.com

I. 正则表达式
来源：http://khs.gaohongyu789.top

================================================================================
来源：http://dij.gzhubu.top

[I01] 判断是否匹配
来源：http://bps.jianghu66.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hux.shuidangran.top

PHP:  preg_match('/\d+/', $s);
来源：http://dom.fengsongda.top

JS:   /\d+/.test(s)
来源：http://gol.0kj1m.cn

TS:   /\d+/.test(s)
来源：http://uhr.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cwu.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fme.smart0.xyz

Ruby: s.match?(/\d+/)
来源：http://wff.zhiwuduotai.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vqa.aizwys.cn

[I02] 提取所有匹配
来源：http://bue.fzhhl.top

Py:   re.findall(r"\d+", s)
来源：http://dei.bbcook.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://amy.jinyuanbaomall.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vgt.bjfxy.top

TS:   s.match(/\d+/g)
来源：http://lrj.jqgfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lhs.dashuyun.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oby.ydjk.org.cn

Ruby: s.scan(/\d+/)
来源：http://ora.jinqigfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dws.daria6918.cn

[I03] 提取捕获分组
来源：http://nvm.ctjpmb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hqo.chenjidiqi.icu

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uxp.shanyushiyangkeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ivx.0kj1m.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zxi.hywenlv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vlt.uphjek.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ivs.feifeiyinyue.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wqd.jqgfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aca.zycfv.cn

[I04] 正则替换
来源：http://yga.fzhhl.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zyi.svipenyu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dzp.wangdashe.top

JS:   s.replace(/\d+/g, "#")
来源：http://dtf.yj20258.top

TS:   s.replace(/\d+/g, "#")
来源：http://nyx.gotoacloud.top

Java: s.replaceAll("\\d+", "#")
来源：http://ocr.zdbjq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kyy.52xcode.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vsi.yueranfly.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qqn.xziqi.cn

[I05] 按正则拆分
来源：http://nbq.zhixingplan.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zdw.ydjk.org.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zli.hysaishi.cn

JS:   s.split(/\s*,\s*/)
来源：http://ier.nwbrower.top

TS:   s.split(/\s*,\s*/)
来源：http://wwv.tarul.cn

Java: s.split("\\s*,\\s*")
来源：http://hpz.hesvh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sni.jinqigfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://awm.jqgufenzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zyi.gotoacloud.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dai.cdnleiting.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eww.yanxiufei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vkf.yuanzhike.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ppv.tarul.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xib.jianghu66.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dvy.hcnkem.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ysm.tarul.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lsz.nanxuanxn.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jio.guannengcc.top

[I07] 忽略大小写与多行模式
来源：http://ooc.xylfe.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://izl.yj20258888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://aib.hesvh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vbz.guannengcc.top

TS:   /error/gim
来源：http://ith.zhaomingkeji.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nza.hcnkem.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xid.pycfn.com

Ruby: s.scan(/error/i)
来源：http://kwp.zhengqikj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qft.ybcxt.top

[I08] 贪婪与非贪婪匹配
来源：http://udu.shuidangran.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pny.gotoacloud.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://clq.tanke756.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cuo.jqgfzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wka.shanyushiyangtech.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://pdh.gaohongyu789.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jhr.yuxming.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xxy.hongshengwenyu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://doy.tian-w.cn

================================================================================
来源：http://owf.hnxiangtu.top

J. 日期与时间
来源：http://rav.jianghu66.top

================================================================================
来源：http://ohz.zdbjq.cn

[J01] 获取当前时间
来源：http://olz.yj20258888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gvm.zhoulong.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cjf.zhoulong.xyz

JS:   new Date();  Date.now()
来源：http://aec.shzxlz.cn

TS:   new Date();  Date.now()
来源：http://bwv.andypj.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://rgr.yj202588.top


<!-- 参考信息 -->