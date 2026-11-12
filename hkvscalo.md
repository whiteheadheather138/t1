代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://gkc.birdmap.top

Ruby: def greet; @name; end
来源：http://ree.yuxming.cn

C#:   public string Greet() => Name;
来源：http://wht.yonumen.top

[G05] 继承
来源：http://ezt.sweek.top

Py:   class Admin(User): pass
来源：http://had.gogol.net.cn

PHP:  class Admin extends User {}
来源：http://dcn.fehbvm.com

JS:   class Admin extends User {}
来源：http://gkr.jianghu66.top

TS:   class Admin extends User {}
来源：http://vtj.sysykeji.top

Java: class Admin extends User {}
来源：http://bch.havefunace.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uyt.cashguo.top

Ruby: class Admin < User; end
来源：http://gxk.ppjwa.cn

C#:   class Admin : User {}
来源：http://hir.sweek.top

[G06] 重写方法
来源：http://lln.nanxinkj.top

Py:   def greet(self): return "admin"
来源：http://aoj.tian-w.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mzu.cashguo.top

JS:   greet() { return "admin"; }
来源：http://jqu.meibo888.top

TS:   greet(): string { return "admin"; }
来源：http://fyv.birdmap.top

Java: @Override String greet() { return "admin"; }
来源：http://fpq.epnwcf.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mre.shanyushiyangkeji.top

Ruby: def greet; "admin"; end
来源：http://zkt.zhongyouzk.top

C#:   public override string Greet() => "admin";
来源：http://hvr.ydzc1.top

[G07] 调用父类方法
来源：http://bcf.feifeiyinyue.top

Py:   super().greet()
来源：http://glb.ivvv.top

PHP:  parent::greet();
来源：http://rnn.bjfxy.top

JS:   super.greet();
来源：http://zgj.ctjpmb.com

TS:   super.greet();
来源：http://vle.sufxvd.cn

Java: super.greet();
来源：http://ycg.wangshuangyany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://koy.aibaodan.cn

Ruby: super
来源：http://crj.ydjk.org.cn

C#:   base.Greet();
来源：http://aqr.jqgufenzy.top

[G08] 静态方法与属性
来源：http://ige.shangyingyoupin.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vme.ivvv.top

PHP:  public static function f() {}
来源：http://xui.tian-w.cn

JS:   static f() {}
来源：http://fqo.zhixingplan.top

TS:   static f(): void {}
来源：http://buc.vehdjk.com

Java: static void f() {}
来源：http://pej.9152youxi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gff.zycfv.cn

Ruby: def self.f; end
来源：http://wrx.9152youxi.cn

C#:   public static void F() {}
来源：http://cuf.ctjpmb.com

[G09] 接口 / 抽象类
来源：http://axt.gotoacloud.top

Py:   from abc import ABC, abstractmethod
来源：http://wfa.snrcjt.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qef.zdbjq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gnp.xuanzx.com

TS:   interface Shape { area(): number; }
来源：http://nsb.sxryk.cn

Java: interface Shape { double area(); }
来源：http://xwp.xylfe.cn

Go:   type Shape interface { Area() float64 }
来源：http://aed.redwolf501.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oqr.yj20258.top

C#:   interface IShape { double Area(); }
来源：http://ozg.zdbjq.cn

[G10] 访问控制
来源：http://lxk.jinghuilouyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://dlg.dashuyun.cn

PHP:  public / protected / private
来源：http://ulj.daria6918.cn

JS:   #private 字段；其余公开
来源：http://ryk.aibaodan.cn

TS:   public / protected / private
来源：http://rxf.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://wjt.xinyue.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://bfy.redwolf501.top

Ruby: public / protected / private
来源：http://uxi.ehwqpu.com

C#:   public / protected / private / internal
来源：http://gub.cucudq.cn

[G11] getter / setter
来源：http://fay.meibo888.top

Py:   @property 与 @x.setter
来源：http://wmc.yangfankeji.com

PHP:  public function getName(): string { return $this->name; }
来源：http://tqb.birdmap.top

JS:   get name() { return this._name; }
来源：http://epg.316326.xyz

TS:   get name(): string { return this._name; }
来源：http://dlt.ydjk.org.cn

Java: public String getName() { return name; }
来源：http://aqx.yuxming.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jvl.yanxiufei.cn

Ruby: attr_accessor :name
来源：http://pwh.iojbl.cn

C#:   public string Name { get; set; }
来源：http://mst.jiagoushi.top

[G12] 对象转字符串
来源：http://nce.xylfe.cn

Py:   def __str__(self): return self.name
来源：http://owr.dashuyun.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://krn.hnxiangtu.top

JS:   toString() { return this.name; }
来源：http://pxx.ybcxt.top

TS:   toString(): string { return this.name; }
来源：http://iqv.fzhhl.top

Java: @Override public String toString() { return name; }
来源：http://ysa.hnxiangtu.top

Go:   func (u User) String() string { return u.Name }
来源：http://ojs.tian-w.cn

Ruby: def to_s; @name; end
来源：http://xqc.hesvh.cn

C#:   public override string ToString() => Name;
来源：http://rqv.shuidangran.top

[G13] 判断对象类型
来源：http://hzy.cucudq.cn

Py:   isinstance(u, User)
来源：http://yjh.hysaishi.cn

PHP:  $u instanceof User
来源：http://lqm.cucudq.cn

JS:   u instanceof User
来源：http://sed.jqgufenzy.top

TS:   u instanceof User
来源：http://zvg.jqgufenzy.top

Java: u instanceof User
来源：http://ysm.chenlongwang.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ffl.fehbvm.com

Ruby: u.is_a?(User)
来源：http://asn.sufxvd.cn

C#:   u is User
来源：http://dsq.hnqzz.top

[G14] 数据类 / record
来源：http://tpw.ehwqpu.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xkf.jiagoushi.top

PHP:  // 用 readonly 属性模拟
来源：http://bje.xingfuxueyuan.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://ipg.yongpay.top

TS:   type User = { name: string; age: number };
来源：http://cdc.zhiwuduotai.top

Java: record User(String name, int age) {}
来源：http://qsk.xylfe.cn

Go:   type User struct { Name string; Age int }
来源：http://ejt.cqqwz.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fxp.bjfxy.top

C#:   record User(string Name, int Age);
来源：http://get.ydjk.org.cn

[G15] 枚举
来源：http://njo.sjlbkw.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pla.ehwqpu.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://tfa.zhengqikj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://spu.epnwcf.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://joh.aibaodan.cn

Java: enum Color { RED, GREEN }
来源：http://skf.sjlbkw.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://izn.xinyue.icu

Ruby: Color = %i[red green].freeze
来源：http://fen.ybcxt.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qho.svipenyu.cn

[G16] 对象转数组 / 字典
来源：http://sjk.yangfankeji.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vzf.nwbrower.top

PHP:  get_object_vars($obj);
来源：http://gmi.guowangkeji.top

JS:   Object.entries(obj)
来源：http://pcm.hfpthk.cn

TS:   Object.entries(obj)
来源：http://exl.aizwys.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://koe.daxiang520.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ghs.guowangkeji.top

Ruby: obj.instance_variables
来源：http://fkh.52xcode.cn

C#:   // 用反射或 System.Text.Json
来源：http://dxx.haohaochexian.top

================================================================================
来源：http://gha.vqdsnc.cn

H. 异常与错误处理
来源：http://jfm.epnwcf.com

================================================================================
来源：http://rtx.fehbvm.com

[H01] try / catch 基础
来源：http://puq.jqgufenzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://krw.vehdjk.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ksj.316326.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pbb.ppjwa.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mfi.cashguo.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fqn.cheryme.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ron.yj20258.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ybg.zhiwuduotai.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vkt.havefunace.top

[H02] finally / ensure 收尾
来源：http://lrx.yanxiufei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ebx.havefunace.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://flt.gaohongyu789.top

JS:   try { f(); } finally { cleanup(); }
来源：http://kbj.jqgfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gys.pycfn.com

Java: try { f(); } finally { cleanup(); }
来源：http://yyg.316326.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://psk.fengsongda.top

Ruby: begin; f; ensure; cleanup; end
来源：http://rgc.sjlbkw.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dzv.sjlbkw.cn

[H03] 主动抛出异常
来源：http://otf.birdmap.top

Py:   raise ValueError("错误信息")
来源：http://pdo.svipenyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vdk.yanxiufei.cn

JS:   throw new Error("错误信息");
来源：http://ufq.hnqzz.top

TS:   throw new Error("错误信息");
来源：http://gxd.hnxiangtu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://gyf.shangyingyoupin.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mal.ydjk.org.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rux.52xcode.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kng.uphjek.com

[H04] 自定义异常类型
来源：http://fqv.jinghuilouyu.cn

Py:   class MyError(Exception): pass
来源：http://rzb.birdmap.top

PHP:  class MyError extends RuntimeException {}
来源：http://avr.tarul.cn

JS:   class MyError extends Error {}
来源：http://fpf.fktsv.cn

TS:   class MyError extends Error {}
来源：http://ore.birdmap.top

Java: class MyException extends RuntimeException {}
来源：http://ebc.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cdx.hfpthk.cn

Ruby: class MyError < StandardError; end
来源：http://oea.jinqigfzy.top

C#:   class MyException : Exception {}
来源：http://fwg.quarkkingdee.top

[H05] 捕获特定类型
来源：http://euq.jlsjyb.cn

Py:   except ValueError as e:
来源：http://qpn.jinqigufen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jbr.zhijiandao.cn

JS:   if (e instanceof TypeError) {}
来源：http://bra.zhengqikj.top

TS:   if (e instanceof TypeError) {}
来源：http://qez.zdbjq.cn

Java: catch (IOException | SQLException e) {}
来源：http://ujz.yongpay.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kpt.fktsv.cn

Ruby: rescue ArgumentError => e
来源：http://fzr.shuidangran.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rug.meibo888.top

[H06] 可选值 / 空值安全访问
来源：http://ocg.snrcjt.cn

Py:   value = d.get("k") or default
来源：http://fiy.epnwcf.com

PHP:  $v = $d["k"] ?? null;
来源：http://gxz.tianlin.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://uud.xinyue.icu

TS:   obj?.a?.b;  d ?? default
来源：http://zni.svipenyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xuh.yongpay.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hap.cheryme.top

Ruby: d&.dig(:a, :b)
来源：http://tul.hammf.cn

C#:   obj?.A?.B ?? default
来源：http://ppd.316326.xyz

[H07] 断言
来源：http://fcs.hnqzz.top

Py:   assert x > 0, "必须为正"
来源：http://rcn.yuxming.cn

PHP:  assert($x > 0);
来源：http://lql.shanyushiyangkeji.top

JS:   console.assert(x > 0);
来源：http://qbo.cheryme.top

TS:   console.assert(x > 0);
来源：http://jde.jianghu66.top

Java: assert x > 0 : "必须为正";
来源：http://ntx.havefunace.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jyw.hywenlv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jzr.redwolf501.top

C#:   Debug.Assert(x > 0);
来源：http://gfp.guannengcc.top

[H08] 获取错误信息与堆栈
来源：http://fnp.jqgufenzy.top

Py:   str(e);  traceback.format_exc()
来源：http://crd.hnqzz.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rjz.xuanzx.com

JS:   e.message;  e.stack
来源：http://amb.xuanzx.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://kac.daria6918.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cjz.zycfv.cn

Go:   err.Error()
来源：http://huj.sufxvd.cn

Ruby: e.message;  e.backtrace
来源：http://klo.hywenlv.cn

C#:   e.Message;  e.StackTrace
来源：http://wli.yueranfly.top

[H09] 带错误码的异常
来源：http://dne.yj202588.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bav.52xcode.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lpl.bjfxy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rqc.shuidangran.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fit.vehdjk.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yri.havefunace.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://feh.yuxming.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yhx.quarkkingdee.top

C#:   // 自定义异常类中加 Code 属性
来源：http://owg.zhengqikj.top

[H10] 资源自动释放
来源：http://dbq.vehdjk.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://nnj.ppjwa.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bcf.fzhhl.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kls.hfpthk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mat.c1oappe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nap.hnxiangtu.top

Go:   defer f.Close()
来源：http://qcg.sufxvd.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uou.chenjidiqi.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kdn.hywenlv.cn

================================================================================
来源：http://vaz.hnxiangtu.top

I. 正则表达式
来源：http://bzv.ehwqpu.com

================================================================================
来源：http://cem.hammf.cn

[I01] 判断是否匹配
来源：http://oap.iojbl.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gao.chenjidiqi.icu

PHP:  preg_match('/\d+/', $s);
来源：http://zpd.xylfe.cn

JS:   /\d+/.test(s)
来源：http://ivh.sweek.top

TS:   /\d+/.test(s)
来源：http://hna.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gmt.pycfn.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jdp.zhaomingkeji.xyz

Ruby: s.match?(/\d+/)
来源：http://jho.haohaochexian.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xkq.chenlongwang.top

[I02] 提取所有匹配
来源：http://emi.mhx1999.top

Py:   re.findall(r"\d+", s)
来源：http://rfj.0kj1m.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ffk.yj20258.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mch.birdmap.top

TS:   s.match(/\d+/g)
来源：http://stx.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yil.fktsv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://itx.ehwqpu.com

Ruby: s.scan(/\d+/)
来源：http://nla.yj20258888.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cdm.jqgfzy.top

[I03] 提取捕获分组
来源：http://uev.cqqwz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uwu.gaohongyu789.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lta.yvedp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://prz.zycfv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://otz.chenzaomai.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tqp.zhijiandao.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cyu.guowangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mec.feifeiyinyue.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://quy.jinqigufen.top

[I04] 正则替换
来源：http://iol.chenzaomai.com

Py:   re.sub(r"\d+", "#", s)
来源：http://wug.gogol.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mxv.jqgfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://ufe.ivvv.top

TS:   s.replace(/\d+/g, "#")
来源：http://fzh.shuidangran.top

Java: s.replaceAll("\\d+", "#")
来源：http://uiz.gzhubu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mxm.zycfv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xlp.wangdashe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rhk.hesvh.cn

[I05] 按正则拆分
来源：http://hol.jlsjyb.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zvj.hnqzz.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://npb.0kj1m.cn

JS:   s.split(/\s*,\s*/)
来源：http://gam.yonumen.top

TS:   s.split(/\s*,\s*/)
来源：http://fck.hysaishi.cn

Java: s.split("\\s*,\\s*")
来源：http://ago.zycfv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ayg.yongpay.top

Ruby: s.split(/\s*,\s*/)
来源：http://xtf.xuetiantiany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://who.yj20258888.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bdu.sjlbkw.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bvo.yonumen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dyd.shanyushiyangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://isd.wangshuangyany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://itb.guannengcc.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oul.fanxiaobao.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uly.gaohongyu789.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lkm.epnwcf.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://txj.haohaochexian.top

[I07] 忽略大小写与多行模式
来源：http://rbl.zhoulong.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://scv.guowangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ept.9152youxi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fsq.xuanzx.com

TS:   /error/gim
来源：http://ruj.hysaishi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vzw.yonumen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mkh.kuanghao11.cn

Ruby: s.scan(/error/i)
来源：http://avb.jyoumei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nnq.tianlin.xyz

[I08] 贪婪与非贪婪匹配
来源：http://xzu.feifeiyinyue.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ikc.chenlongwang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lkg.dashuyun.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ekw.fehbvm.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xfc.gzhubu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://tie.zdqjudy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tbd.aizwys.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nwm.fengsongda.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xjn.hywenlv.cn

================================================================================
来源：http://cls.yj202588.top

J. 日期与时间
来源：http://lno.feifeiyinyue.top

================================================================================
来源：http://tyc.havefunace.top

[J01] 获取当前时间
来源：http://zdg.jinqigfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://lyl.epnwcf.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://way.yfazqb.com

JS:   new Date();  Date.now()
来源：http://rxw.sjlbkw.cn

TS:   new Date();  Date.now()
来源：http://hqt.hcnkem.com

Java: LocalDateTime.now();  Instant.now()
来源：http://qos.0kj1m.cn

Go:   time.Now()
来源：http://bkr.ctjpmb.com

Ruby: Time.now
来源：http://xsk.sweek.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bpg.cashguo.top

[J02] 格式化输出
来源：http://huv.cqqwz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://spo.guannengcc.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ssj.aizwys.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qww.feifeiyinyue.top

TS:   d.toISOString()
来源：http://nyj.cqqwz.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nfu.ctjpmb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://owf.hfpthk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rce.yvedp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yyr.jqgfzy.top


<!-- 参考信息 -->