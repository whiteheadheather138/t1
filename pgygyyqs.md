代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://mmt.xziqi.cn

[G07] 调用父类方法
来源：http://vvc.jlsjyb.cn

Py:   super().greet()
来源：http://tuy.tianlin.xyz

PHP:  parent::greet();
来源：http://fxf.pycfn.com

JS:   super.greet();
来源：http://sxh.chenzaomai.com

TS:   super.greet();
来源：http://zbr.snrcjt.cn

Java: super.greet();
来源：http://ytk.yj202588.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ver.gzhubu.top

Ruby: super
来源：http://zqt.pycfn.com

C#:   base.Greet();
来源：http://vjf.yongpay.top

[G08] 静态方法与属性
来源：http://lrc.nwbrower.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://esb.ydzc1.top

PHP:  public static function f() {}
来源：http://oug.sysykeji.top

JS:   static f() {}
来源：http://fbq.hfpthk.cn

TS:   static f(): void {}
来源：http://xui.shuidangran.top

Java: static void f() {}
来源：http://zbr.sjlbkw.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rvc.hywenlv.cn

Ruby: def self.f; end
来源：http://dmy.zdqjudy.top

C#:   public static void F() {}
来源：http://zqf.sjlbkw.cn

[G09] 接口 / 抽象类
来源：http://yka.vqdsnc.cn

Py:   from abc import ABC, abstractmethod
来源：http://znb.yj202588.top

PHP:  interface Shape { public function area(): float; }
来源：http://mjv.jinqigfzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://paa.daxiang520.top

TS:   interface Shape { area(): number; }
来源：http://lci.yangfankeji.com

Java: interface Shape { double area(); }
来源：http://dpq.bjfxy.top

Go:   type Shape interface { Area() float64 }
来源：http://qhs.xuanzx.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qln.xuetiantiany.cn

C#:   interface IShape { double Area(); }
来源：http://qzi.chenjidiqi.icu

[G10] 访问控制
来源：http://nod.yueranfly.top

Py:   约定 _protected / __private（不强制）
来源：http://ept.sysykeji.top

PHP:  public / protected / private
来源：http://qfh.pycfn.com

JS:   #private 字段；其余公开
来源：http://yup.hnxiangtu.top

TS:   public / protected / private
来源：http://crk.sysykeji.top

Java: public / protected / private / 默认包级
来源：http://vnw.shanyushiyangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://khi.yuanzhike.top

Ruby: public / protected / private
来源：http://eou.gogol.net.cn

C#:   public / protected / private / internal
来源：http://cvj.fehbvm.com

[G11] getter / setter
来源：http://blu.kuanghao11.cn

Py:   @property 与 @x.setter
来源：http://img.yuxming.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yzl.cashguo.top

JS:   get name() { return this._name; }
来源：http://zsn.svipenyu.cn

TS:   get name(): string { return this._name; }
来源：http://nze.ivvv.top

Java: public String getName() { return name; }
来源：http://gze.xuanzx.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://boa.cqqwz.cn

Ruby: attr_accessor :name
来源：http://icc.shzxlz.cn

C#:   public string Name { get; set; }
来源：http://pwf.jinqigfzy.top

[G12] 对象转字符串
来源：http://txf.jinqigfzy.top

Py:   def __str__(self): return self.name
来源：http://nth.xingfuxueyuan.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://xhw.wangdashe.top

JS:   toString() { return this.name; }
来源：http://wxr.zhongyouzk.top

TS:   toString(): string { return this.name; }
来源：http://lal.xingfuxueyuan.xyz

Java: @Override public String toString() { return name; }
来源：http://kra.ppjwa.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ymu.aizwys.cn

Ruby: def to_s; @name; end
来源：http://plu.bbcook.cn

C#:   public override string ToString() => Name;
来源：http://uam.c1oappe.top

[G13] 判断对象类型
来源：http://giz.bjfxy.top

Py:   isinstance(u, User)
来源：http://sol.52xcode.cn

PHP:  $u instanceof User
来源：http://uln.xylfe.cn

JS:   u instanceof User
来源：http://nei.meibo888.top

TS:   u instanceof User
来源：http://ewu.feifeiyinyue.top

Java: u instanceof User
来源：http://kjh.xziqi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fjx.jqgufenzy.top

Ruby: u.is_a?(User)
来源：http://hak.quarkkingdee.top

C#:   u is User
来源：http://tng.nwbrower.top

[G14] 数据类 / record
来源：http://ivj.pycfn.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xjr.ybcxt.top

PHP:  // 用 readonly 属性模拟
来源：http://wlw.0kj1m.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qgr.pycfn.com

TS:   type User = { name: string; age: number };
来源：http://nwx.daria6918.cn

Java: record User(String name, int age) {}
来源：http://dqr.jqgfzy.top

Go:   type User struct { Name string; Age int }
来源：http://ogg.tarul.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sko.hammf.cn

C#:   record User(string Name, int Age);
来源：http://hba.xuanzx.com

[G15] 枚举
来源：http://ffc.iojbl.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cvg.shuidangran.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xmy.cdnleiting.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yrn.dianchejie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ctv.jiagoushi.top

Java: enum Color { RED, GREEN }
来源：http://ete.ctjpmb.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hwu.zhengqikj.top

Ruby: Color = %i[red green].freeze
来源：http://sck.smart0.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://feq.9152youxi.cn

[G16] 对象转数组 / 字典
来源：http://adf.hysaishi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tpe.hfpthk.cn

PHP:  get_object_vars($obj);
来源：http://ksb.meibo888.top

JS:   Object.entries(obj)
来源：http://qzz.yanxiufei.cn

TS:   Object.entries(obj)
来源：http://okn.xuetiantiany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://stk.bjfxy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gss.pycfn.com

Ruby: obj.instance_variables
来源：http://eue.jinghuilouyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://ali.nwbrower.top

================================================================================
来源：http://dod.hnqzz.top

H. 异常与错误处理
来源：http://pvo.jlsjyb.cn

================================================================================
来源：http://ryz.yongpay.top

[H01] try / catch 基础
来源：http://ckp.sufxvd.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ztx.aibaodan.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ttr.hnqzz.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mbv.hnxiangtu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cuq.aizwys.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fph.shangyingyoupin.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://eoq.yj202588.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jvo.yj20258.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uia.hcnkem.com

[H02] finally / ensure 收尾
来源：http://aak.0kj1m.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wfi.hnqzz.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ihk.zycfv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vum.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://byo.jinqigufen.top

Java: try { f(); } finally { cleanup(); }
来源：http://gxm.yuanzhike.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://yxe.hnqzz.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qho.smart0.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://emt.ehwqpu.com

[H03] 主动抛出异常
来源：http://kvl.jqgufenzy.top

Py:   raise ValueError("错误信息")
来源：http://myp.bjfxy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zvk.jinyuanbaomall.cn

JS:   throw new Error("错误信息");
来源：http://xuy.hysaishi.cn

TS:   throw new Error("错误信息");
来源：http://naf.zhiwuduotai.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jvv.yfazqb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ynw.52xcode.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://squ.0kj1m.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mxn.hnqzz.top

[H04] 自定义异常类型
来源：http://hbx.zhongyouzk.top

Py:   class MyError(Exception): pass
来源：http://bfh.xinyue.icu

PHP:  class MyError extends RuntimeException {}
来源：http://ums.yangfankeji.com

JS:   class MyError extends Error {}
来源：http://ckc.jinyuanbaomall.cn

TS:   class MyError extends Error {}
来源：http://hlg.ydjk.org.cn

Java: class MyException extends RuntimeException {}
来源：http://ylp.cdnleiting.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zro.gogol.net.cn

Ruby: class MyError < StandardError; end
来源：http://xsz.cucudq.cn

C#:   class MyException : Exception {}
来源：http://tpu.xinyue.icu

[H05] 捕获特定类型
来源：http://hkn.tanke756.top

Py:   except ValueError as e:
来源：http://fmr.cqqwz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qyc.gzhubu.top

JS:   if (e instanceof TypeError) {}
来源：http://kbv.tarul.cn

TS:   if (e instanceof TypeError) {}
来源：http://okf.jinghuilouyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://omm.yanxiufei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uqp.nanxinkj.top

Ruby: rescue ArgumentError => e
来源：http://pap.jianghu66.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wlg.hywenlv.cn

[H06] 可选值 / 空值安全访问
来源：http://amv.9152youxi.cn

Py:   value = d.get("k") or default
来源：http://gvb.jianghu66.top

PHP:  $v = $d["k"] ?? null;
来源：http://vpf.gaohongyu789.top

JS:   obj?.a?.b;  d ?? default
来源：http://put.hnxiangtu.top

TS:   obj?.a?.b;  d ?? default
来源：http://qml.bjfxy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ecs.tianlin.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://mal.zhoulong.xyz

Ruby: d&.dig(:a, :b)
来源：http://vwl.gzhubu.top

C#:   obj?.A?.B ?? default
来源：http://zwf.cashguo.top

[H07] 断言
来源：http://dmb.yvedp.cn

Py:   assert x > 0, "必须为正"
来源：http://ejn.hywenlv.cn

PHP:  assert($x > 0);
来源：http://npv.shzxlz.cn

JS:   console.assert(x > 0);
来源：http://vwr.jqgfzy.top

TS:   console.assert(x > 0);
来源：http://nqv.xingfuxueyuan.xyz

Java: assert x > 0 : "必须为正";
来源：http://iaj.wangdashe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cwk.jianghu66.top

Ruby: raise "必须为正" unless x > 0
来源：http://hfb.guowangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://cio.meibo888.top

[H08] 获取错误信息与堆栈
来源：http://upw.ydzc1.top

Py:   str(e);  traceback.format_exc()
来源：http://bcf.daria6918.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bxp.snrcjt.cn

JS:   e.message;  e.stack
来源：http://drh.wangshuangyany.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kjb.fengsongda.top

Java: e.getMessage();  e.printStackTrace()
来源：http://hoa.yanxiufei.cn

Go:   err.Error()
来源：http://xql.hysaishi.cn

Ruby: e.message;  e.backtrace
来源：http://ikq.kuanghao11.cn

C#:   e.Message;  e.StackTrace
来源：http://xuk.zhongyouzk.top

[H09] 带错误码的异常
来源：http://yll.uphjek.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bgo.fengsongda.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rad.wangshuangyany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zga.jiagoushi.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ahe.jqgfzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yxc.cucudq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gmo.shangyingyoupin.top

Ruby: raise MyError.new("fail", 500)
来源：http://ggi.gaohongyu789.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ryv.wangdashe.top

[H10] 资源自动释放
来源：http://fcs.gogol.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mvi.fktsv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://egm.jinqigfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ieu.svipenyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xfn.zhixingplan.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://crz.52xcode.cn

Go:   defer f.Close()
来源：http://vhr.jiagoushi.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sqe.hesvh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wlo.ehwqpu.com

================================================================================
来源：http://jyv.fzhhl.top

I. 正则表达式
来源：http://qfi.meibo888.top

================================================================================
来源：http://zsk.chenjidiqi.icu

[I01] 判断是否匹配
来源：http://nsl.fanxiaobao.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mng.c1oappe.top

PHP:  preg_match('/\d+/', $s);
来源：http://ugc.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://uuj.daxiang520.top

TS:   /\d+/.test(s)
来源：http://sid.jiagoushi.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mlb.zhengqikj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vgq.fanxiaobao.xyz

Ruby: s.match?(/\d+/)
来源：http://idc.hongshengwenyu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uir.zhengqikj.top

[I02] 提取所有匹配
来源：http://epf.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://hav.aizwys.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://idi.hongshengwenyu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rfr.tian-w.cn

TS:   s.match(/\d+/g)
来源：http://upx.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://igj.bjfxy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jul.tanke756.top

Ruby: s.scan(/\d+/)
来源：http://vrn.haohaochexian.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fnr.ydzc1.top

[I03] 提取捕获分组
来源：http://tfr.fzhhl.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xnl.cucudq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rwj.yfazqb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lig.tanke756.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://muc.hnqzz.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://aaq.xziqi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gvs.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://urc.c1oappe.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iup.jiagoushi.top

[I04] 正则替换
来源：http://dzn.jlsjyb.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xts.yanxiufei.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mdj.tarul.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ukx.fengsongda.top

TS:   s.replace(/\d+/g, "#")
来源：http://zhm.9152youxi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qgc.xuanzx.com

Go:   re.ReplaceAllString(s, "#")
来源：http://vqh.feifeiyinyue.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vze.epnwcf.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ebx.yanxiufei.cn

[I05] 按正则拆分
来源：http://ztx.ctjpmb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://bzy.jianghu66.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mlj.chenzaomai.com

JS:   s.split(/\s*,\s*/)
来源：http://qva.jinyuanbaomall.cn

TS:   s.split(/\s*,\s*/)
来源：http://wei.vqdsnc.cn

Java: s.split("\\s*,\\s*")
来源：http://zdf.pengpengdd.cyou

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eqe.jiagoushi.top

Ruby: s.split(/\s*,\s*/)
来源：http://vqq.ywan-chungtsiang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pce.jinqigufen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ogc.dianchejie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mfb.fengsongda.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ruv.gzhubu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rnq.c1oappe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xbd.pycfn.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wxd.cheryme.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eah.meibo888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://orq.hcnkem.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jfw.hnxiangtu.top

[I07] 忽略大小写与多行模式
来源：http://hlg.jinghuilouyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fyd.jinqigfzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://chq.bbcook.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fhb.zhiwuduotai.top

TS:   /error/gim
来源：http://bsm.xingfuxueyuan.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wub.yueranfly.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rso.xuetiantiany.cn

Ruby: s.scan(/error/i)
来源：http://tgl.redwolf501.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://grn.zhaomingkeji.xyz

[I08] 贪婪与非贪婪匹配
来源：http://fcu.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fgu.mhx1999.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ghm.cheryme.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ebe.tarul.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uqr.hysaishi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qic.fengsongda.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vgz.ydjk.org.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rkb.sxryk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://atg.sufxvd.cn

================================================================================
来源：http://uxr.ivvv.top

J. 日期与时间
来源：http://bds.zhijiandao.cn

================================================================================
来源：http://kqs.316326.xyz

[J01] 获取当前时间
来源：http://hpl.cashguo.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zgu.cdnleiting.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mjr.yuanzhike.top

JS:   new Date();  Date.now()
来源：http://ptl.jinghuilouyu.cn

TS:   new Date();  Date.now()
来源：http://ioa.aibaodan.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ito.nanxinkj.top

Go:   time.Now()
来源：http://wbi.9152youxi.cn

Ruby: Time.now
来源：http://lqs.fehbvm.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pya.zhongyouzk.top

[J02] 格式化输出
来源：http://ukr.yfazqb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ipt.nwbrower.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yuw.xziqi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bse.316326.xyz

TS:   d.toISOString()
来源：http://zid.jyoumei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rhq.uphjek.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zxz.wangdashe.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pdc.gaohongyu789.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qus.zhoulong.xyz

[J03] 字符串解析为日期
来源：http://yhe.ydjk.org.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://icm.nanxinkj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dsn.sufxvd.cn

JS:   new Date("2024-01-02")
来源：http://jwq.aibaodan.cn

TS:   new Date("2024-01-02")
来源：http://erw.yj20258.top

Java: LocalDate.parse("2024-01-02")
来源：http://cum.yuanzhike.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://evm.xylfe.cn

Ruby: Date.parse("2024-01-02")
来源：http://ves.epnwcf.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://osb.dashuyun.cn

[J04] 时间戳与日期互转
来源：http://otz.pycfn.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xpw.jiagoushi.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tgj.ppjwa.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wsn.vehdjk.com

TS:   Math.floor(Date.now() / 1000)
来源：http://orl.vehdjk.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hgo.aizwys.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fgk.zhongyouzk.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qpz.jiagoushi.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eqd.tarul.cn

[J05] 时间加减（加 7 天）
来源：http://ykq.zhijiandao.cn

Py:   now + timedelta(days=7)
来源：http://elc.hesvh.cn


<!-- 参考信息 -->