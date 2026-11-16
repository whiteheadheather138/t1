代发 wailian999

Java: class Admin extends User {}
来源：http://lyg.nwbrower.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lny.nwbrower.top

Ruby: class Admin < User; end
来源：http://jve.sjlbkw.cn

C#:   class Admin : User {}
来源：http://zay.yuanzhike.top

[G06] 重写方法
来源：http://icw.daria6918.cn

Py:   def greet(self): return "admin"
来源：http://yvx.yanxiufei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pce.gotoacloud.top

JS:   greet() { return "admin"; }
来源：http://ips.zhijiandao.cn

TS:   greet(): string { return "admin"; }
来源：http://fxa.zhongyouzk.top

Java: @Override String greet() { return "admin"; }
来源：http://iuy.0kj1m.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nne.redwolf501.top

Ruby: def greet; "admin"; end
来源：http://lnu.andypj.xyz

C#:   public override string Greet() => "admin";
来源：http://gjm.hesvh.cn

[G07] 调用父类方法
来源：http://ntg.ehwqpu.com

Py:   super().greet()
来源：http://tnb.hnxiangtu.top

PHP:  parent::greet();
来源：http://kjv.haohaochexian.top

JS:   super.greet();
来源：http://qun.meibo888.top

TS:   super.greet();
来源：http://bsj.dashuyun.cn

Java: super.greet();
来源：http://voj.sysykeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tzr.fanxiaobao.xyz

Ruby: super
来源：http://oce.ywan-chungtsiang.top

C#:   base.Greet();
来源：http://xtj.meibo888.top

[G08] 静态方法与属性
来源：http://omw.uphjek.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ifp.yuanzhike.top

PHP:  public static function f() {}
来源：http://xho.cdnleiting.top

JS:   static f() {}
来源：http://yxh.yueranfly.top

TS:   static f(): void {}
来源：http://xav.gzhubu.top

Java: static void f() {}
来源：http://aue.gotoacloud.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://pao.hnqzz.top

Ruby: def self.f; end
来源：http://pwv.pycfn.com

C#:   public static void F() {}
来源：http://lbz.snrcjt.cn

[G09] 接口 / 抽象类
来源：http://nwe.quarkkingdee.top

Py:   from abc import ABC, abstractmethod
来源：http://yga.zhiwuduotai.top

PHP:  interface Shape { public function area(): float; }
来源：http://jam.hcnkem.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://nvn.hnqzz.top

TS:   interface Shape { area(): number; }
来源：http://uud.smart0.xyz

Java: interface Shape { double area(); }
来源：http://biz.quarkkingdee.top

Go:   type Shape interface { Area() float64 }
来源：http://pwa.xinyue.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gdt.zhongyouzk.top

C#:   interface IShape { double Area(); }
来源：http://hcd.kuanghao11.cn

[G10] 访问控制
来源：http://wiq.zdqjudy.top

Py:   约定 _protected / __private（不强制）
来源：http://jra.quarkkingdee.top

PHP:  public / protected / private
来源：http://hse.52xcode.cn

JS:   #private 字段；其余公开
来源：http://rmi.bjfxy.top

TS:   public / protected / private
来源：http://xmj.nwbrower.top

Java: public / protected / private / 默认包级
来源：http://hvh.pengpengdd.cyou

Go:   首字母大写可导出，小写仅包内可见
来源：http://bfa.ehwqpu.com

Ruby: public / protected / private
来源：http://oet.tarul.cn

C#:   public / protected / private / internal
来源：http://cnr.tanke756.top

[G11] getter / setter
来源：http://rro.andypj.xyz

Py:   @property 与 @x.setter
来源：http://xwt.yangfankeji.com

PHP:  public function getName(): string { return $this->name; }
来源：http://nlw.gaohongyu789.top

JS:   get name() { return this._name; }
来源：http://rkd.0kj1m.cn

TS:   get name(): string { return this._name; }
来源：http://nne.hcnkem.com

Java: public String getName() { return name; }
来源：http://jlp.hysaishi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ltx.tian-w.cn

Ruby: attr_accessor :name
来源：http://sgw.uphjek.com

C#:   public string Name { get; set; }
来源：http://wec.zhiwuduotai.top

[G12] 对象转字符串
来源：http://tdb.gogol.net.cn

Py:   def __str__(self): return self.name
来源：http://mex.gogol.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://stb.zdbjq.cn

JS:   toString() { return this.name; }
来源：http://uyw.jinqigfzy.top

TS:   toString(): string { return this.name; }
来源：http://qgo.chenlongwang.top

Java: @Override public String toString() { return name; }
来源：http://kew.yonumen.top

Go:   func (u User) String() string { return u.Name }
来源：http://zmb.birdmap.top

Ruby: def to_s; @name; end
来源：http://yrm.tanke756.top

C#:   public override string ToString() => Name;
来源：http://zmc.iojbl.cn

[G13] 判断对象类型
来源：http://mjn.nanxuanxn.top

Py:   isinstance(u, User)
来源：http://moi.316326.xyz

PHP:  $u instanceof User
来源：http://qov.sweek.top

JS:   u instanceof User
来源：http://iih.zdqjudy.top

TS:   u instanceof User
来源：http://nvd.ydzc1.top

Java: u instanceof User
来源：http://yrq.ydjk.org.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lcz.uphjek.com

Ruby: u.is_a?(User)
来源：http://uax.jiagoushi.top

C#:   u is User
来源：http://xlp.yueranfly.top

[G14] 数据类 / record
来源：http://igk.c1oappe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tkq.wangdashe.top

PHP:  // 用 readonly 属性模拟
来源：http://dmk.tianlin.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://uqp.pycfn.com

TS:   type User = { name: string; age: number };
来源：http://vox.vehdjk.com

Java: record User(String name, int age) {}
来源：http://adt.jyoumei.cn

Go:   type User struct { Name string; Age int }
来源：http://kbt.sxryk.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://erg.yonumen.top

C#:   record User(string Name, int Age);
来源：http://swx.yj20258.top

[G15] 枚举
来源：http://spq.birdmap.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://odt.ctjpmb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://xfd.birdmap.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xqt.zycfv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hgi.chenzaomai.com

Java: enum Color { RED, GREEN }
来源：http://qtf.pycfn.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nbb.andypj.xyz

Ruby: Color = %i[red green].freeze
来源：http://jac.yongpay.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dws.xuetiantiany.cn

[G16] 对象转数组 / 字典
来源：http://nti.tanke756.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vwo.gzhubu.top

PHP:  get_object_vars($obj);
来源：http://cpk.yvedp.cn

JS:   Object.entries(obj)
来源：http://ikd.wangdashe.top

TS:   Object.entries(obj)
来源：http://suy.cucudq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://njb.yuxming.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rbd.guannengcc.top

Ruby: obj.instance_variables
来源：http://nsz.wangshuangyany.cn

C#:   // 用反射或 System.Text.Json
来源：http://woj.jinyuanbaomall.cn

================================================================================
来源：http://uzi.shanyushiyangkeji.top

H. 异常与错误处理
来源：http://hlo.xuanzx.com

================================================================================
来源：http://mwv.bjfxy.top

[H01] try / catch 基础
来源：http://jpe.yj20258888.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sqz.ybcxt.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rwd.snrcjt.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qao.wangdashe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://abr.zhiwuduotai.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hpk.gotoacloud.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jca.cheryme.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tui.zhoulong.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pdf.c1oappe.top

[H02] finally / ensure 收尾
来源：http://qpy.feifeiyinyue.top

Py:   try: f()⏎finally: cleanup()
来源：http://fhr.sysykeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://edv.cdnleiting.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ggb.wangshuangyany.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cpb.hammf.cn

Java: try { f(); } finally { cleanup(); }
来源：http://akr.cheryme.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://soa.snrcjt.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lnr.ctjpmb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://yuo.yangfankeji.com

[H03] 主动抛出异常
来源：http://rlc.wangdashe.top

Py:   raise ValueError("错误信息")
来源：http://yzk.zhengqikj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qgk.gogol.net.cn

JS:   throw new Error("错误信息");
来源：http://qnq.xinyue.icu

TS:   throw new Error("错误信息");
来源：http://tse.fzhhl.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ifx.9152youxi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://agl.sjlbkw.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rkf.tian-w.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wqs.iojbl.cn

[H04] 自定义异常类型
来源：http://zso.daria6918.cn

Py:   class MyError(Exception): pass
来源：http://lsf.shanyushiyangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://ikh.fzhhl.top

JS:   class MyError extends Error {}
来源：http://qym.hesvh.cn

TS:   class MyError extends Error {}
来源：http://jye.dashuyun.cn

Java: class MyException extends RuntimeException {}
来源：http://cqm.tanke756.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tba.gotoacloud.top

Ruby: class MyError < StandardError; end
来源：http://afw.ywan-chungtsiang.top

C#:   class MyException : Exception {}
来源：http://rxz.daxiang520.top

[H05] 捕获特定类型
来源：http://bpu.yuxming.cn

Py:   except ValueError as e:
来源：http://khx.yangfankeji.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jlw.yueranfly.top

JS:   if (e instanceof TypeError) {}
来源：http://flj.smart0.xyz

TS:   if (e instanceof TypeError) {}
来源：http://hoo.dashuyun.cn

Java: catch (IOException | SQLException e) {}
来源：http://oaj.52xcode.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cnn.tian-w.cn

Ruby: rescue ArgumentError => e
来源：http://fho.uphjek.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zke.ctjpmb.com

[H06] 可选值 / 空值安全访问
来源：http://vvq.jqgfzy.top

Py:   value = d.get("k") or default
来源：http://vfd.yuxming.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jbe.shanyushiyangtech.top

JS:   obj?.a?.b;  d ?? default
来源：http://lfn.zycfv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vls.sufxvd.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dym.yj202588.top

Go:   if v, ok := m["k"]; ok { }
来源：http://mjk.cdnleiting.top

Ruby: d&.dig(:a, :b)
来源：http://cco.zhengqikj.top

C#:   obj?.A?.B ?? default
来源：http://pld.ydjk.org.cn

[H07] 断言
来源：http://lnp.xylfe.cn

Py:   assert x > 0, "必须为正"
来源：http://egf.uphjek.com

PHP:  assert($x > 0);
来源：http://maa.epnwcf.com

JS:   console.assert(x > 0);
来源：http://toc.nanxinkj.top

TS:   console.assert(x > 0);
来源：http://jns.gogol.net.cn

Java: assert x > 0 : "必须为正";
来源：http://ybw.nanxuanxn.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nlr.vehdjk.com

Ruby: raise "必须为正" unless x > 0
来源：http://rzs.guannengcc.top

C#:   Debug.Assert(x > 0);
来源：http://osv.daria6918.cn

[H08] 获取错误信息与堆栈
来源：http://plb.snrcjt.cn

Py:   str(e);  traceback.format_exc()
来源：http://yol.jinyuanbaomall.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mpp.dashuyun.cn

JS:   e.message;  e.stack
来源：http://cmy.52xcode.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qrr.gaohongyu789.top

Java: e.getMessage();  e.printStackTrace()
来源：http://avk.ehwqpu.com

Go:   err.Error()
来源：http://pki.hnxiangtu.top

Ruby: e.message;  e.backtrace
来源：http://tbz.wangdashe.top

C#:   e.Message;  e.StackTrace
来源：http://gcr.jlsjyb.cn

[H09] 带错误码的异常
来源：http://bvq.yuxming.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dgm.quarkkingdee.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://cmp.yuxming.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qig.jyoumei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ulm.wangdashe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fbe.jyoumei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ovv.zhongyouzk.top

Ruby: raise MyError.new("fail", 500)
来源：http://iix.fzhhl.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jbz.bbcook.cn

[H10] 资源自动释放
来源：http://sir.yj20258.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://bhm.ppjwa.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ics.sysykeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ymh.jqgfzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dun.xinyue.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://iwt.ctjpmb.com

Go:   defer f.Close()
来源：http://ojv.fktsv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fbf.wangshuangyany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eao.guannengcc.top

================================================================================
来源：http://rfv.shangyingyoupin.top

I. 正则表达式
来源：http://nau.xylfe.cn

================================================================================
来源：http://gwb.aizwys.cn

[I01] 判断是否匹配
来源：http://wot.guannengcc.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lju.tarul.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qzx.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://oqm.shanyushiyangkeji.top

TS:   /\d+/.test(s)
来源：http://qtq.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nvq.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ksv.jinyuanbaomall.cn

Ruby: s.match?(/\d+/)
来源：http://wyg.yj20258888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://msh.meibo888.top

[I02] 提取所有匹配
来源：http://qku.yueranfly.top

Py:   re.findall(r"\d+", s)
来源：http://lrx.ivvv.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uhn.0kj1m.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sne.fengsongda.top

TS:   s.match(/\d+/g)
来源：http://smj.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nrg.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tfk.zhiwuduotai.top

Ruby: s.scan(/\d+/)
来源：http://dtf.xinyue.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://aao.aibaodan.cn

[I03] 提取捕获分组
来源：http://jkh.mhx1999.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rsq.chenlongwang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zxm.daria6918.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wki.sysykeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rae.zhongyouzk.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gsm.shangyingyoupin.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://arl.jyoumei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cps.fengsongda.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://liu.fehbvm.com

[I04] 正则替换
来源：http://wsh.gzhubu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://iai.yj20258.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fha.yuanzhike.top

JS:   s.replace(/\d+/g, "#")
来源：http://uwg.xziqi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ojx.mhx1999.top

Java: s.replaceAll("\\d+", "#")
来源：http://kfj.xinyue.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://mzl.tanke756.top

Ruby: s.gsub(/\d+/, "#")
来源：http://btm.fanxiaobao.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gkx.jiagoushi.top

[I05] 按正则拆分
来源：http://uzo.316326.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://zxf.jinqigufen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cwd.xinyue.icu

JS:   s.split(/\s*,\s*/)
来源：http://jmy.ydjk.org.cn

TS:   s.split(/\s*,\s*/)
来源：http://nca.fengsongda.top

Java: s.split("\\s*,\\s*")
来源：http://jbk.yonumen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cxe.ppjwa.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jkc.gotoacloud.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hkr.jqgfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xpf.vehdjk.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eni.xingfuxueyuan.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xvn.vehdjk.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kdk.hfpthk.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ffo.hesvh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zbd.hnxiangtu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gaa.yuxming.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wjy.xziqi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tdt.ywan-chungtsiang.top

[I07] 忽略大小写与多行模式
来源：http://ffw.bjfxy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qzg.hywenlv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tfn.yvedp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rvr.nwbrower.top

TS:   /error/gim
来源：http://fmd.jinyuanbaomall.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ini.hysaishi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://reo.fengsongda.top

Ruby: s.scan(/error/i)
来源：http://oxf.wangdashe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dee.yfazqb.com

[I08] 贪婪与非贪婪匹配
来源：http://laa.vqdsnc.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mkd.tanke756.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lcb.9152youxi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pfw.tarul.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nvm.ivvv.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mhv.jinyuanbaomall.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qia.fktsv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://enw.bjfxy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dhj.jqgfzy.top

================================================================================
来源：http://dsj.ivvv.top

J. 日期与时间
来源：http://swg.shanyushiyangkeji.top

================================================================================
来源：http://asb.sjlbkw.cn

[J01] 获取当前时间
来源：http://ibl.yj20258888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xuw.ydjk.org.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nre.yfazqb.com

JS:   new Date();  Date.now()
来源：http://hyv.zhiwuduotai.top

TS:   new Date();  Date.now()
来源：http://qqd.ybcxt.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dji.jlsjyb.cn

Go:   time.Now()
来源：http://mqv.jinyuanbaomall.cn

Ruby: Time.now
来源：http://tcf.jlsjyb.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gny.zhoulong.xyz

[J02] 格式化输出
来源：http://dvx.fehbvm.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ywa.redwolf501.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://azo.quarkkingdee.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cwz.hnqzz.top

TS:   d.toISOString()
来源：http://jzf.hysaishi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kmx.sxryk.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://teq.yj20258888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://svq.hysaishi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sbe.pycfn.com

[J03] 字符串解析为日期
来源：http://wko.yvedp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ivq.hfpthk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ixz.cucudq.cn

JS:   new Date("2024-01-02")
来源：http://ldb.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://mho.cheryme.top

Java: LocalDate.parse("2024-01-02")
来源：http://tay.guannengcc.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nzf.nanxuanxn.top

Ruby: Date.parse("2024-01-02")
来源：http://fth.gaohongyu789.top


<!-- 参考信息 -->