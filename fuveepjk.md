代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://zyh.haohaochexian.top

Java: @Override String greet() { return "admin"; }
来源：http://ayx.jyoumei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fmt.daxiang520.top

Ruby: def greet; "admin"; end
来源：http://xrs.zhongyouzk.top

C#:   public override string Greet() => "admin";
来源：http://qjl.fzhhl.top

[G07] 调用父类方法
来源：http://pqm.zhaomingkeji.xyz

Py:   super().greet()
来源：http://kaq.tarul.cn

PHP:  parent::greet();
来源：http://hak.jinyuanbaomall.cn

JS:   super.greet();
来源：http://tet.hnxiangtu.top

TS:   super.greet();
来源：http://bdq.wangshuangyany.cn

Java: super.greet();
来源：http://rtq.yangfankeji.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lkk.zhiwuduotai.top

Ruby: super
来源：http://yul.jianghu66.top

C#:   base.Greet();
来源：http://peg.svipenyu.cn

[G08] 静态方法与属性
来源：http://psa.epnwcf.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ymk.andypj.xyz

PHP:  public static function f() {}
来源：http://pah.jinyuanbaomall.cn

JS:   static f() {}
来源：http://zgz.cheryme.top

TS:   static f(): void {}
来源：http://lsm.shangyingyoupin.top

Java: static void f() {}
来源：http://gvp.ctjpmb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://fsu.nwbrower.top

Ruby: def self.f; end
来源：http://zoh.fanxiaobao.xyz

C#:   public static void F() {}
来源：http://ddq.shanyushiyangtech.top

[G09] 接口 / 抽象类
来源：http://zpg.havefunace.top

Py:   from abc import ABC, abstractmethod
来源：http://ddf.pycfn.com

PHP:  interface Shape { public function area(): float; }
来源：http://mud.gaohongyu789.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://owb.epnwcf.com

TS:   interface Shape { area(): number; }
来源：http://pwo.52xcode.cn

Java: interface Shape { double area(); }
来源：http://dik.fanxiaobao.xyz

Go:   type Shape interface { Area() float64 }
来源：http://sit.shanyushiyangtech.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ydw.iojbl.cn

C#:   interface IShape { double Area(); }
来源：http://dzb.fktsv.cn

[G10] 访问控制
来源：http://ego.jinqigfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://qhu.hongshengwenyu.top

PHP:  public / protected / private
来源：http://ymh.meibo888.top

JS:   #private 字段；其余公开
来源：http://rnq.0kj1m.cn

TS:   public / protected / private
来源：http://dst.yangfankeji.com

Java: public / protected / private / 默认包级
来源：http://nue.fktsv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vex.epnwcf.com

Ruby: public / protected / private
来源：http://jrz.bjfxy.top

C#:   public / protected / private / internal
来源：http://ybs.gogol.net.cn

[G11] getter / setter
来源：http://fzx.cheryme.top

Py:   @property 与 @x.setter
来源：http://dsa.redwolf501.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bil.havefunace.top

JS:   get name() { return this._name; }
来源：http://mzt.wangdashe.top

TS:   get name(): string { return this._name; }
来源：http://vgb.shanyushiyangtech.top

Java: public String getName() { return name; }
来源：http://rff.sxryk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cio.0kj1m.cn

Ruby: attr_accessor :name
来源：http://kys.chenzaomai.com

C#:   public string Name { get; set; }
来源：http://vaw.shangyingyoupin.top

[G12] 对象转字符串
来源：http://win.bbcook.cn

Py:   def __str__(self): return self.name
来源：http://wre.bjfxy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://dow.cheryme.top

JS:   toString() { return this.name; }
来源：http://cwb.zdbjq.cn

TS:   toString(): string { return this.name; }
来源：http://hzt.jinqigufen.top

Java: @Override public String toString() { return name; }
来源：http://wln.jinqigfzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://spj.andypj.xyz

Ruby: def to_s; @name; end
来源：http://tws.ehwqpu.com

C#:   public override string ToString() => Name;
来源：http://utu.hfpthk.cn

[G13] 判断对象类型
来源：http://fct.daria6918.cn

Py:   isinstance(u, User)
来源：http://zrf.andypj.xyz

PHP:  $u instanceof User
来源：http://qtd.yj20258888.top

JS:   u instanceof User
来源：http://pjr.aizwys.cn

TS:   u instanceof User
来源：http://vdo.tian-w.cn

Java: u instanceof User
来源：http://tjz.xylfe.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bio.cucudq.cn

Ruby: u.is_a?(User)
来源：http://xld.jlsjyb.cn

C#:   u is User
来源：http://stj.nwbrower.top

[G14] 数据类 / record
来源：http://qig.gogol.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ana.c1oappe.top

PHP:  // 用 readonly 属性模拟
来源：http://onj.redwolf501.top

JS:   // 无内置：普通类或对象字面量
来源：http://kgj.316326.xyz

TS:   type User = { name: string; age: number };
来源：http://qhg.hongshengwenyu.top

Java: record User(String name, int age) {}
来源：http://gzj.kuanghao11.cn

Go:   type User struct { Name string; Age int }
来源：http://wpr.ydjk.org.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://aqv.0kj1m.cn

C#:   record User(string Name, int Age);
来源：http://kfr.ctjpmb.com

[G15] 枚举
来源：http://lot.gotoacloud.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lax.fktsv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wsd.ivvv.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lgs.zhongyouzk.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://awg.hnqzz.top

Java: enum Color { RED, GREEN }
来源：http://dax.aizwys.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dba.cashguo.top

Ruby: Color = %i[red green].freeze
来源：http://ngf.fzhhl.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fxu.yuxming.cn

[G16] 对象转数组 / 字典
来源：http://mub.shanyushiyangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://udc.hcnkem.com

PHP:  get_object_vars($obj);
来源：http://xxt.daria6918.cn

JS:   Object.entries(obj)
来源：http://jiw.guowangkeji.top

TS:   Object.entries(obj)
来源：http://izb.hysaishi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://eqj.ehwqpu.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://muj.zycfv.cn

Ruby: obj.instance_variables
来源：http://asn.vehdjk.com

C#:   // 用反射或 System.Text.Json
来源：http://unm.gogol.net.cn

================================================================================
来源：http://esx.yonumen.top

H. 异常与错误处理
来源：http://qeo.wangshuangyany.cn

================================================================================
来源：http://xpz.yonumen.top

[H01] try / catch 基础
来源：http://lyy.tian-w.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hqf.yongpay.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oqm.jinqigfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wtq.feifeiyinyue.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yvv.tanke756.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gkn.feifeiyinyue.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wmy.xziqi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xff.svipenyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lor.zhengqikj.top

[H02] finally / ensure 收尾
来源：http://bra.cashguo.top

Py:   try: f()⏎finally: cleanup()
来源：http://egi.ctjpmb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://mzn.52xcode.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ubs.zhengqikj.top

TS:   try { f(); } finally { cleanup(); }
来源：http://umv.jqgfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://mas.zhijiandao.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yds.0kj1m.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fhf.zycfv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ghv.ppjwa.cn

[H03] 主动抛出异常
来源：http://znn.bbcook.cn

Py:   raise ValueError("错误信息")
来源：http://ghc.jinyuanbaomall.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gxq.cdnleiting.top

JS:   throw new Error("错误信息");
来源：http://iye.shangyingyoupin.top

TS:   throw new Error("错误信息");
来源：http://mtz.cashguo.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://sls.bbcook.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zpl.bbcook.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kje.fzhhl.top

C#:   throw new ArgumentException("错误信息");
来源：http://xxd.cheryme.top

[H04] 自定义异常类型
来源：http://djt.chenlongwang.top

Py:   class MyError(Exception): pass
来源：http://fjp.jqgufenzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://fge.cashguo.top

JS:   class MyError extends Error {}
来源：http://tsd.yongpay.top

TS:   class MyError extends Error {}
来源：http://may.zycfv.cn

Java: class MyException extends RuntimeException {}
来源：http://nre.yonumen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eyw.vehdjk.com

Ruby: class MyError < StandardError; end
来源：http://geb.xingfuxueyuan.xyz

C#:   class MyException : Exception {}
来源：http://cen.jqgfzy.top

[H05] 捕获特定类型
来源：http://ofg.pycfn.com

Py:   except ValueError as e:
来源：http://eix.hcnkem.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mzv.fehbvm.com

JS:   if (e instanceof TypeError) {}
来源：http://ztu.bjfxy.top

TS:   if (e instanceof TypeError) {}
来源：http://dcw.zhengqikj.top

Java: catch (IOException | SQLException e) {}
来源：http://rci.pengpengdd.cyou

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hme.zycfv.cn

Ruby: rescue ArgumentError => e
来源：http://wax.smart0.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iox.hcnkem.com

[H06] 可选值 / 空值安全访问
来源：http://xza.tarul.cn

Py:   value = d.get("k") or default
来源：http://rpu.zhiwuduotai.top

PHP:  $v = $d["k"] ?? null;
来源：http://tgr.yvedp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://njy.jinqigfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://msz.nwbrower.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lnh.hnqzz.top

Go:   if v, ok := m["k"]; ok { }
来源：http://isg.ivvv.top

Ruby: d&.dig(:a, :b)
来源：http://sfi.bbcook.cn

C#:   obj?.A?.B ?? default
来源：http://ztm.mhx1999.top

[H07] 断言
来源：http://bkx.gaohongyu789.top

Py:   assert x > 0, "必须为正"
来源：http://zke.ehwqpu.com

PHP:  assert($x > 0);
来源：http://pvi.yangfankeji.com

JS:   console.assert(x > 0);
来源：http://shb.fehbvm.com

TS:   console.assert(x > 0);
来源：http://ouk.jinghuilouyu.cn

Java: assert x > 0 : "必须为正";
来源：http://rnm.zhijiandao.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gyi.hnqzz.top

Ruby: raise "必须为正" unless x > 0
来源：http://akx.bjfxy.top

C#:   Debug.Assert(x > 0);
来源：http://mdb.xziqi.cn

[H08] 获取错误信息与堆栈
来源：http://eyx.quarkkingdee.top

Py:   str(e);  traceback.format_exc()
来源：http://tup.wangdashe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ncc.ydjk.org.cn

JS:   e.message;  e.stack
来源：http://yyd.yj20258.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://dra.vqdsnc.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wxp.ehwqpu.com

Go:   err.Error()
来源：http://kel.hnqzz.top

Ruby: e.message;  e.backtrace
来源：http://opn.shanyushiyangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://wdk.feifeiyinyue.top

[H09] 带错误码的异常
来源：http://ihz.ehwqpu.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jps.sxryk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://exn.meibo888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://syk.meibo888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://una.sysykeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dae.shzxlz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jrp.daria6918.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pkt.fehbvm.com

C#:   // 自定义异常类中加 Code 属性
来源：http://ksd.iojbl.cn

[H10] 资源自动释放
来源：http://aqv.yueranfly.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dyd.jinyuanbaomall.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://phh.jinqigufen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ulj.pycfn.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jrt.mhx1999.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rnt.hfpthk.cn

Go:   defer f.Close()
来源：http://vvg.cucudq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://eoc.jqgufenzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eey.tianlin.xyz

================================================================================
来源：http://uxy.gaohongyu789.top

I. 正则表达式
来源：http://hxk.yuxming.cn

================================================================================
来源：http://kyn.zdbjq.cn

[I01] 判断是否匹配
来源：http://chg.zdqjudy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://txf.epnwcf.com

PHP:  preg_match('/\d+/', $s);
来源：http://ruu.sweek.top

JS:   /\d+/.test(s)
来源：http://bdg.nwbrower.top

TS:   /\d+/.test(s)
来源：http://ngv.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ghd.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lbv.shanyushiyangtech.top

Ruby: s.match?(/\d+/)
来源：http://zyt.yonumen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gcy.cdnleiting.top

[I02] 提取所有匹配
来源：http://uwd.yj20258.top

Py:   re.findall(r"\d+", s)
来源：http://tlp.yuxming.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cqk.chenjidiqi.icu

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mwg.pengpengdd.cyou

TS:   s.match(/\d+/g)
来源：http://qks.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://eaj.c1oappe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zwd.jinyuanbaomall.cn

Ruby: s.scan(/\d+/)
来源：http://jqx.hysaishi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nfo.zhijiandao.cn

[I03] 提取捕获分组
来源：http://udj.daxiang520.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://laf.wangshuangyany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mzo.hcnkem.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xyy.zdqjudy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ouf.snrcjt.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kyl.snrcjt.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://utf.zycfv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pym.fktsv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://utw.tianlin.xyz

[I04] 正则替换
来源：http://blt.xuanzx.com

Py:   re.sub(r"\d+", "#", s)
来源：http://wcv.hywenlv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ial.yuanzhike.top

JS:   s.replace(/\d+/g, "#")
来源：http://wcm.ybcxt.top

TS:   s.replace(/\d+/g, "#")
来源：http://szw.andypj.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://jmw.sufxvd.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rpb.jyoumei.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ssn.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yct.zdbjq.cn

[I05] 按正则拆分
来源：http://jis.gaohongyu789.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xoo.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://aoq.nanxinkj.top

JS:   s.split(/\s*,\s*/)
来源：http://jsa.nanxinkj.top

TS:   s.split(/\s*,\s*/)
来源：http://ijf.pycfn.com

Java: s.split("\\s*,\\s*")
来源：http://hpy.zdbjq.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fej.guowangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://idi.haohaochexian.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qkd.hfpthk.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vbx.zhaomingkeji.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qgq.yueranfly.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://svo.yuxming.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xxv.zhixingplan.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aom.tarul.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tgp.chenzaomai.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lxr.xziqi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pak.yj20258.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ctu.shangyingyoupin.top

[I07] 忽略大小写与多行模式
来源：http://lkq.zycfv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qab.snrcjt.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gbe.xingfuxueyuan.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mfl.wangshuangyany.cn

TS:   /error/gim
来源：http://gvm.vehdjk.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cva.guannengcc.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rvp.tanke756.top

Ruby: s.scan(/error/i)
来源：http://rse.pycfn.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mel.jinqigufen.top

[I08] 贪婪与非贪婪匹配
来源：http://ooi.guannengcc.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zlm.nanxinkj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wce.jqgfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ofc.ctjpmb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://leu.hongshengwenyu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://izc.zhiwuduotai.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eui.zdbjq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rnz.sweek.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bdr.shanyushiyangtech.top

================================================================================
来源：http://mio.yuanzhike.top

J. 日期与时间
来源：http://ray.vehdjk.com

================================================================================
来源：http://xgw.yanxiufei.cn

[J01] 获取当前时间
来源：http://ibw.vehdjk.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://wov.zdbjq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zev.iojbl.cn

JS:   new Date();  Date.now()
来源：http://hce.uphjek.com

TS:   new Date();  Date.now()
来源：http://hrg.svipenyu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ezo.c1oappe.top

Go:   time.Now()
来源：http://nty.snrcjt.cn

Ruby: Time.now
来源：http://ldz.cqqwz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://omu.hammf.cn

[J02] 格式化输出
来源：http://rfi.snrcjt.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vlt.cheryme.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gke.sweek.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iqx.yj20258.top

TS:   d.toISOString()
来源：http://nxn.zhixingplan.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dwj.0kj1m.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://okl.ydjk.org.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mnm.ivvv.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vwv.hnqzz.top

[J03] 字符串解析为日期
来源：http://ztn.sjlbkw.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://umz.pycfn.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pxa.yj202588.top

JS:   new Date("2024-01-02")
来源：http://zik.yuxming.cn

TS:   new Date("2024-01-02")
来源：http://wck.nanxuanxn.top

Java: LocalDate.parse("2024-01-02")
来源：http://cjw.yongpay.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wca.yvedp.cn

Ruby: Date.parse("2024-01-02")
来源：http://onh.shuidangran.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ncv.snrcjt.cn

[J04] 时间戳与日期互转
来源：http://hgr.kuanghao11.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bss.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bxa.sufxvd.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ibl.xylfe.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ccx.hnqzz.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://anr.yuxming.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cad.hammf.cn


<!-- 参考信息 -->