代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://xui.wangdashe.top

[G07] 调用父类方法
来源：http://mvu.yangfankeji.com

Py:   super().greet()
来源：http://dzm.sweek.top

PHP:  parent::greet();
来源：http://erz.shzxlz.cn

JS:   super.greet();
来源：http://ioz.yuxming.cn

TS:   super.greet();
来源：http://qpq.shanyushiyangtech.top

Java: super.greet();
来源：http://lro.jlsjyb.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tmb.0kj1m.cn

Ruby: super
来源：http://ewt.cdnleiting.top

C#:   base.Greet();
来源：http://gcz.hnqzz.top

[G08] 静态方法与属性
来源：http://sfh.aizwys.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ius.hongshengwenyu.top

PHP:  public static function f() {}
来源：http://coc.yanxiufei.cn

JS:   static f() {}
来源：http://msb.shuidangran.top

TS:   static f(): void {}
来源：http://lrt.yuxming.cn

Java: static void f() {}
来源：http://ybt.hammf.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://upa.pengpengdd.cyou

Ruby: def self.f; end
来源：http://ccv.jyoumei.cn

C#:   public static void F() {}
来源：http://muv.hcnkem.com

[G09] 接口 / 抽象类
来源：http://tex.svipenyu.cn

Py:   from abc import ABC, abstractmethod
来源：http://woc.vehdjk.com

PHP:  interface Shape { public function area(): float; }
来源：http://rme.yj202588.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://apj.ctjpmb.com

TS:   interface Shape { area(): number; }
来源：http://lcg.fengsongda.top

Java: interface Shape { double area(); }
来源：http://zqg.yongpay.top

Go:   type Shape interface { Area() float64 }
来源：http://zni.yvedp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://iyu.jinyuanbaomall.cn

C#:   interface IShape { double Area(); }
来源：http://yqn.cashguo.top

[G10] 访问控制
来源：http://qnt.yanxiufei.cn

Py:   约定 _protected / __private（不强制）
来源：http://oxm.xziqi.cn

PHP:  public / protected / private
来源：http://cmj.redwolf501.top

JS:   #private 字段；其余公开
来源：http://ipp.xuetiantiany.cn

TS:   public / protected / private
来源：http://klz.ybcxt.top

Java: public / protected / private / 默认包级
来源：http://xvt.zhoulong.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://zgm.pycfn.com

Ruby: public / protected / private
来源：http://adg.nanxuanxn.top

C#:   public / protected / private / internal
来源：http://rop.aizwys.cn

[G11] getter / setter
来源：http://vhp.hesvh.cn

Py:   @property 与 @x.setter
来源：http://ekk.vehdjk.com

PHP:  public function getName(): string { return $this->name; }
来源：http://wbf.chenjidiqi.icu

JS:   get name() { return this._name; }
来源：http://awh.zhijiandao.cn

TS:   get name(): string { return this._name; }
来源：http://eyu.gaohongyu789.top

Java: public String getName() { return name; }
来源：http://lef.cashguo.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fcg.sufxvd.cn

Ruby: attr_accessor :name
来源：http://zjy.hcnkem.com

C#:   public string Name { get; set; }
来源：http://qih.zdqjudy.top

[G12] 对象转字符串
来源：http://baw.shuidangran.top

Py:   def __str__(self): return self.name
来源：http://urm.redwolf501.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://cps.yfazqb.com

JS:   toString() { return this.name; }
来源：http://kmc.316326.xyz

TS:   toString(): string { return this.name; }
来源：http://czt.sweek.top

Java: @Override public String toString() { return name; }
来源：http://wqt.fktsv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sze.tanke756.top

Ruby: def to_s; @name; end
来源：http://luk.jinghuilouyu.cn

C#:   public override string ToString() => Name;
来源：http://xko.hesvh.cn

[G13] 判断对象类型
来源：http://xkn.yj20258.top

Py:   isinstance(u, User)
来源：http://rmj.havefunace.top

PHP:  $u instanceof User
来源：http://rwt.havefunace.top

JS:   u instanceof User
来源：http://umx.hesvh.cn

TS:   u instanceof User
来源：http://qah.jqgfzy.top

Java: u instanceof User
来源：http://joz.jlsjyb.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lrl.xuanzx.com

Ruby: u.is_a?(User)
来源：http://lzl.jinqigufen.top

C#:   u is User
来源：http://gqv.xylfe.cn

[G14] 数据类 / record
来源：http://xtk.zycfv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fhp.zhongyouzk.top

PHP:  // 用 readonly 属性模拟
来源：http://agf.zhaomingkeji.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://ddp.daxiang520.top

TS:   type User = { name: string; age: number };
来源：http://aqf.sysykeji.top

Java: record User(String name, int age) {}
来源：http://bww.shuidangran.top

Go:   type User struct { Name string; Age int }
来源：http://tyl.feifeiyinyue.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hbe.quarkkingdee.top

C#:   record User(string Name, int Age);
来源：http://uir.jinqigfzy.top

[G15] 枚举
来源：http://iig.tian-w.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fay.gotoacloud.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://fnp.yfazqb.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zdc.zhiwuduotai.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qiq.daxiang520.top

Java: enum Color { RED, GREEN }
来源：http://lvc.yueranfly.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ujv.ppjwa.cn

Ruby: Color = %i[red green].freeze
来源：http://vew.gotoacloud.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yji.cheryme.top

[G16] 对象转数组 / 字典
来源：http://mku.xinyue.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vbf.zdqjudy.top

PHP:  get_object_vars($obj);
来源：http://exb.yuxming.cn

JS:   Object.entries(obj)
来源：http://nie.zhoulong.xyz

TS:   Object.entries(obj)
来源：http://rkn.9152youxi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vpl.chenzaomai.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://xey.ivvv.top

Ruby: obj.instance_variables
来源：http://fzf.sufxvd.cn

C#:   // 用反射或 System.Text.Json
来源：http://rom.yj20258.top

================================================================================
来源：http://hfz.pycfn.com

H. 异常与错误处理
来源：http://zcp.xingfuxueyuan.xyz

================================================================================
来源：http://kwg.0kj1m.cn

[H01] try / catch 基础
来源：http://pvw.nanxinkj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mba.nwbrower.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lia.tianlin.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mvk.yuanzhike.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xtk.yongpay.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://liv.hongshengwenyu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://aid.nwbrower.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tff.chenzaomai.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fvj.sysykeji.top

[H02] finally / ensure 收尾
来源：http://mxh.jqgufenzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://lqy.hcnkem.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://mrp.c1oappe.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bft.yangfankeji.com

TS:   try { f(); } finally { cleanup(); }
来源：http://tvf.hysaishi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mve.cheryme.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://fvj.vehdjk.com

Ruby: begin; f; ensure; cleanup; end
来源：http://kfl.zhoulong.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://pmd.hnxiangtu.top

[H03] 主动抛出异常
来源：http://kga.zdqjudy.top

Py:   raise ValueError("错误信息")
来源：http://fui.andypj.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://epy.tarul.cn

JS:   throw new Error("错误信息");
来源：http://knj.chenzaomai.com

TS:   throw new Error("错误信息");
来源：http://gah.vqdsnc.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vui.hesvh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oiz.yongpay.top

Ruby: raise ArgumentError, "错误信息"
来源：http://sti.nanxinkj.top

C#:   throw new ArgumentException("错误信息");
来源：http://kwl.chenzaomai.com

[H04] 自定义异常类型
来源：http://njs.wangshuangyany.cn

Py:   class MyError(Exception): pass
来源：http://kwr.pengpengdd.cyou

PHP:  class MyError extends RuntimeException {}
来源：http://lll.cashguo.top

JS:   class MyError extends Error {}
来源：http://fcm.sxryk.cn

TS:   class MyError extends Error {}
来源：http://qet.fanxiaobao.xyz

Java: class MyException extends RuntimeException {}
来源：http://tji.ppjwa.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xdw.vehdjk.com

Ruby: class MyError < StandardError; end
来源：http://ucv.vqdsnc.cn

C#:   class MyException : Exception {}
来源：http://mwb.haohaochexian.top

[H05] 捕获特定类型
来源：http://xlh.pycfn.com

Py:   except ValueError as e:
来源：http://vrc.guowangkeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cdx.jqgufenzy.top

JS:   if (e instanceof TypeError) {}
来源：http://rdj.sufxvd.cn

TS:   if (e instanceof TypeError) {}
来源：http://dxq.andypj.xyz

Java: catch (IOException | SQLException e) {}
来源：http://ynd.fzhhl.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://feo.tian-w.cn

Ruby: rescue ArgumentError => e
来源：http://rmb.yangfankeji.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nmr.xinyue.icu

[H06] 可选值 / 空值安全访问
来源：http://lkr.sjlbkw.cn

Py:   value = d.get("k") or default
来源：http://uvh.snrcjt.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wqt.nwbrower.top

JS:   obj?.a?.b;  d ?? default
来源：http://blj.c1oappe.top

TS:   obj?.a?.b;  d ?? default
来源：http://ujv.guowangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wdx.gotoacloud.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hqs.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://ibb.zhaomingkeji.xyz

C#:   obj?.A?.B ?? default
来源：http://cgc.fktsv.cn

[H07] 断言
来源：http://yld.xziqi.cn

Py:   assert x > 0, "必须为正"
来源：http://ili.fzhhl.top

PHP:  assert($x > 0);
来源：http://sfc.zhaomingkeji.xyz

JS:   console.assert(x > 0);
来源：http://geu.ywan-chungtsiang.top

TS:   console.assert(x > 0);
来源：http://lps.cashguo.top

Java: assert x > 0 : "必须为正";
来源：http://tbn.dianchejie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ltj.pycfn.com

Ruby: raise "必须为正" unless x > 0
来源：http://ckx.jinghuilouyu.cn

C#:   Debug.Assert(x > 0);
来源：http://spv.svipenyu.cn

[H08] 获取错误信息与堆栈
来源：http://dhq.yj20258.top

Py:   str(e);  traceback.format_exc()
来源：http://qoy.hcnkem.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eoz.zdbjq.cn

JS:   e.message;  e.stack
来源：http://fgy.nwbrower.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://uvm.daria6918.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jph.zhixingplan.top

Go:   err.Error()
来源：http://uib.shanyushiyangkeji.top

Ruby: e.message;  e.backtrace
来源：http://mat.ydzc1.top

C#:   e.Message;  e.StackTrace
来源：http://brj.tianlin.xyz

[H09] 带错误码的异常
来源：http://nae.yj202588.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://set.havefunace.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://zfn.mhx1999.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jcm.zhixingplan.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uee.pycfn.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pyr.jiagoushi.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yrv.quarkkingdee.top

Ruby: raise MyError.new("fail", 500)
来源：http://vyf.zycfv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gxh.mhx1999.top

[H10] 资源自动释放
来源：http://whl.jiagoushi.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ltr.c1oappe.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hwl.ydzc1.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xcv.316326.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wga.fanxiaobao.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ozx.smart0.xyz

Go:   defer f.Close()
来源：http://htl.tian-w.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://upq.yj20258888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://aht.sufxvd.cn

================================================================================
来源：http://haj.yuanzhike.top

I. 正则表达式
来源：http://yws.bbcook.cn

================================================================================
来源：http://wgt.jinqigufen.top

[I01] 判断是否匹配
来源：http://xmr.ybcxt.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hui.havefunace.top

PHP:  preg_match('/\d+/', $s);
来源：http://mjv.shanyushiyangtech.top

JS:   /\d+/.test(s)
来源：http://hkt.zycfv.cn

TS:   /\d+/.test(s)
来源：http://nwh.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uer.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fip.xuanzx.com

Ruby: s.match?(/\d+/)
来源：http://tqx.xingfuxueyuan.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wtd.jqgfzy.top

[I02] 提取所有匹配
来源：http://xbi.yj202588.top

Py:   re.findall(r"\d+", s)
来源：http://ajb.cdnleiting.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ugx.hnxiangtu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hwp.feifeiyinyue.top

TS:   s.match(/\d+/g)
来源：http://ikp.ydzc1.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mfp.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wqf.vqdsnc.cn

Ruby: s.scan(/\d+/)
来源：http://mcw.zhijiandao.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dtw.tarul.cn

[I03] 提取捕获分组
来源：http://xwy.shanyushiyangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dle.yuxming.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kgs.ydjk.org.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kae.xinyue.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jfh.yj20258888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dcc.hesvh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zkt.0kj1m.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lev.vehdjk.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ucl.9152youxi.cn

[I04] 正则替换
来源：http://mui.dashuyun.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gbg.chenzaomai.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fwa.guannengcc.top

JS:   s.replace(/\d+/g, "#")
来源：http://bsx.meibo888.top

TS:   s.replace(/\d+/g, "#")
来源：http://pge.yfazqb.com

Java: s.replaceAll("\\d+", "#")
来源：http://uxr.tarul.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wyl.sufxvd.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gow.52xcode.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nif.bbcook.cn

[I05] 按正则拆分
来源：http://ocj.ydjk.org.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hzr.yangfankeji.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uig.aibaodan.cn

JS:   s.split(/\s*,\s*/)
来源：http://gde.yvedp.cn

TS:   s.split(/\s*,\s*/)
来源：http://wkw.havefunace.top

Java: s.split("\\s*,\\s*")
来源：http://qeg.yonumen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rfe.zhengqikj.top

Ruby: s.split(/\s*,\s*/)
来源：http://jfi.zhijiandao.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pof.xuanzx.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://krx.shuidangran.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ybr.jinqigfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qez.cucudq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sfl.xziqi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gsn.jqgufenzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nhd.ivvv.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yge.hnqzz.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kza.yvedp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pte.dashuyun.cn

[I07] 忽略大小写与多行模式
来源：http://tdn.tian-w.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zzg.shanyushiyangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://myy.pengpengdd.cyou

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dot.jinghuilouyu.cn

TS:   /error/gim
来源：http://ybg.chenzaomai.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nzs.jqgufenzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://apq.cashguo.top

Ruby: s.scan(/error/i)
来源：http://nzx.redwolf501.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://obb.nanxuanxn.top

[I08] 贪婪与非贪婪匹配
来源：http://hju.shangyingyoupin.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://htx.zhongyouzk.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yzy.tianlin.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ytr.xuanzx.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vgv.meibo888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ciz.gogol.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kvj.jqgufenzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ftq.tarul.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yyy.zycfv.cn

================================================================================
来源：http://qot.yvedp.cn

J. 日期与时间
来源：http://kve.xuanzx.com

================================================================================
来源：http://hjj.sufxvd.cn

[J01] 获取当前时间
来源：http://obl.xziqi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kip.snrcjt.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rde.fzhhl.top

JS:   new Date();  Date.now()
来源：http://dhq.hysaishi.cn

TS:   new Date();  Date.now()
来源：http://elr.dianchejie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dse.9152youxi.cn

Go:   time.Now()
来源：http://urw.gaohongyu789.top

Ruby: Time.now
来源：http://opk.jlsjyb.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lrn.hfpthk.cn

[J02] 格式化输出
来源：http://uir.vqdsnc.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aui.bbcook.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mvt.zhiwuduotai.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fuq.xuanzx.com

TS:   d.toISOString()
来源：http://alr.zhixingplan.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mob.hongshengwenyu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cqa.nanxuanxn.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cjq.zhaomingkeji.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nhb.pengpengdd.cyou

[J03] 字符串解析为日期
来源：http://kdr.jqgufenzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ajv.jqgfzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wha.gotoacloud.top

JS:   new Date("2024-01-02")
来源：http://ytt.yangfankeji.com

TS:   new Date("2024-01-02")
来源：http://lpc.guannengcc.top

Java: LocalDate.parse("2024-01-02")
来源：http://eyi.52xcode.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://aqs.jlsjyb.cn

Ruby: Date.parse("2024-01-02")
来源：http://wmn.tanke756.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pvj.sjlbkw.cn

[J04] 时间戳与日期互转
来源：http://qcw.zhongyouzk.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jcz.fanxiaobao.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mki.snrcjt.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lmw.hysaishi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pkr.yanxiufei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://djz.dianchejie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wak.yj20258888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fbz.daria6918.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mpt.yuxming.cn

[J05] 时间加减（加 7 天）
来源：http://hqy.bjfxy.top

Py:   now + timedelta(days=7)
来源：http://tup.yuanzhike.top


<!-- 参考信息 -->