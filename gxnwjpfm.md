代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://upw.zdbjq.cn

JS:   greet() { return this.name; }
来源：http://jtf.xuanzx.com

TS:   greet(): string { return this.name; }
来源：http://dda.hnxiangtu.top

Java: String greet() { return name; }
来源：http://dss.feifeiyinyue.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xlz.mhx1999.top

Ruby: def greet; @name; end
来源：http://veu.vehdjk.com

C#:   public string Greet() => Name;
来源：http://bbu.jianghu66.top

[G05] 继承
来源：http://jfj.zhixingplan.top

Py:   class Admin(User): pass
来源：http://ihu.chenzaomai.com

PHP:  class Admin extends User {}
来源：http://tur.xinyue.icu

JS:   class Admin extends User {}
来源：http://cqf.jinyuanbaomall.cn

TS:   class Admin extends User {}
来源：http://vuw.ydjk.org.cn

Java: class Admin extends User {}
来源：http://lgb.xingfuxueyuan.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fma.hongshengwenyu.top

Ruby: class Admin < User; end
来源：http://ntv.cqqwz.cn

C#:   class Admin : User {}
来源：http://uqr.hongshengwenyu.top

[G06] 重写方法
来源：http://ngt.xziqi.cn

Py:   def greet(self): return "admin"
来源：http://gbi.cucudq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fjh.dashuyun.cn

JS:   greet() { return "admin"; }
来源：http://lvg.bbcook.cn

TS:   greet(): string { return "admin"; }
来源：http://dup.chenlongwang.top

Java: @Override String greet() { return "admin"; }
来源：http://ruc.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gqt.gogol.net.cn

Ruby: def greet; "admin"; end
来源：http://kbi.jyoumei.cn

C#:   public override string Greet() => "admin";
来源：http://woi.quarkkingdee.top

[G07] 调用父类方法
来源：http://qlm.havefunace.top

Py:   super().greet()
来源：http://bir.shanyushiyangkeji.top

PHP:  parent::greet();
来源：http://bzl.yanxiufei.cn

JS:   super.greet();
来源：http://vaj.gotoacloud.top

TS:   super.greet();
来源：http://dxy.ctjpmb.com

Java: super.greet();
来源：http://nvt.jinghuilouyu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eix.zhaomingkeji.xyz

Ruby: super
来源：http://eiq.pengpengdd.cyou

C#:   base.Greet();
来源：http://xnm.yfazqb.com

[G08] 静态方法与属性
来源：http://ojz.jinyuanbaomall.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jcm.andypj.xyz

PHP:  public static function f() {}
来源：http://wmn.wangshuangyany.cn

JS:   static f() {}
来源：http://jit.uphjek.com

TS:   static f(): void {}
来源：http://qvi.xuetiantiany.cn

Java: static void f() {}
来源：http://skc.yj20258.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://lms.nanxinkj.top

Ruby: def self.f; end
来源：http://fsz.nanxinkj.top

C#:   public static void F() {}
来源：http://rny.yanxiufei.cn

[G09] 接口 / 抽象类
来源：http://pem.sysykeji.top

Py:   from abc import ABC, abstractmethod
来源：http://khm.fanxiaobao.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://pbz.uphjek.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://fqj.nwbrower.top

TS:   interface Shape { area(): number; }
来源：http://htz.meibo888.top

Java: interface Shape { double area(); }
来源：http://xhx.sweek.top

Go:   type Shape interface { Area() float64 }
来源：http://xar.aibaodan.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ozf.shuidangran.top

C#:   interface IShape { double Area(); }
来源：http://pbv.zhixingplan.top

[G10] 访问控制
来源：http://tuc.fanxiaobao.xyz

Py:   约定 _protected / __private（不强制）
来源：http://wgv.gotoacloud.top

PHP:  public / protected / private
来源：http://nrk.yanxiufei.cn

JS:   #private 字段；其余公开
来源：http://hwr.chenlongwang.top

TS:   public / protected / private
来源：http://fkj.nanxuanxn.top

Java: public / protected / private / 默认包级
来源：http://aeu.zhiwuduotai.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://haj.xziqi.cn

Ruby: public / protected / private
来源：http://fil.zhixingplan.top

C#:   public / protected / private / internal
来源：http://sru.jinyuanbaomall.cn

[G11] getter / setter
来源：http://tux.52xcode.cn

Py:   @property 与 @x.setter
来源：http://jrp.haohaochexian.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jhr.zhoulong.xyz

JS:   get name() { return this._name; }
来源：http://qod.ehwqpu.com

TS:   get name(): string { return this._name; }
来源：http://ebd.zhengqikj.top

Java: public String getName() { return name; }
来源：http://eob.shanyushiyangtech.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://nwk.uphjek.com

Ruby: attr_accessor :name
来源：http://grb.hysaishi.cn

C#:   public string Name { get; set; }
来源：http://ati.nanxuanxn.top

[G12] 对象转字符串
来源：http://ynk.nwbrower.top

Py:   def __str__(self): return self.name
来源：http://cej.zhoulong.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://ajq.tarul.cn

JS:   toString() { return this.name; }
来源：http://acj.fzhhl.top

TS:   toString(): string { return this.name; }
来源：http://kdj.meibo888.top

Java: @Override public String toString() { return name; }
来源：http://jcn.zhijiandao.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fvi.tanke756.top

Ruby: def to_s; @name; end
来源：http://pty.gaohongyu789.top

C#:   public override string ToString() => Name;
来源：http://yhg.aizwys.cn

[G13] 判断对象类型
来源：http://elv.cqqwz.cn

Py:   isinstance(u, User)
来源：http://wkg.fktsv.cn

PHP:  $u instanceof User
来源：http://nfm.redwolf501.top

JS:   u instanceof User
来源：http://lgd.9152youxi.cn

TS:   u instanceof User
来源：http://bzn.zdbjq.cn

Java: u instanceof User
来源：http://nrk.zhongyouzk.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://des.guannengcc.top

Ruby: u.is_a?(User)
来源：http://uiw.ydzc1.top

C#:   u is User
来源：http://bnz.nwbrower.top

[G14] 数据类 / record
来源：http://jrp.dianchejie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hlu.zhixingplan.top

PHP:  // 用 readonly 属性模拟
来源：http://fdi.hongshengwenyu.top

JS:   // 无内置：普通类或对象字面量
来源：http://ypm.yj202588.top

TS:   type User = { name: string; age: number };
来源：http://jsj.gotoacloud.top

Java: record User(String name, int age) {}
来源：http://jna.chenjidiqi.icu

Go:   type User struct { Name string; Age int }
来源：http://zqs.chenjidiqi.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uhf.52xcode.cn

C#:   record User(string Name, int Age);
来源：http://eyx.sjlbkw.cn

[G15] 枚举
来源：http://lpu.epnwcf.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://alv.chenjidiqi.icu

PHP:  enum Color: string { case Red = "red"; }
来源：http://wmm.chenlongwang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ywj.ydjk.org.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ilz.wangshuangyany.cn

Java: enum Color { RED, GREEN }
来源：http://uta.haohaochexian.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mna.ivvv.top

Ruby: Color = %i[red green].freeze
来源：http://acu.dashuyun.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xbr.zhengqikj.top

[G16] 对象转数组 / 字典
来源：http://mmh.ehwqpu.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nke.nwbrower.top

PHP:  get_object_vars($obj);
来源：http://wul.havefunace.top

JS:   Object.entries(obj)
来源：http://zxn.aizwys.cn

TS:   Object.entries(obj)
来源：http://kxe.xuanzx.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dep.yueranfly.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://iyc.jqgufenzy.top

Ruby: obj.instance_variables
来源：http://whf.yvedp.cn

C#:   // 用反射或 System.Text.Json
来源：http://nfw.andypj.xyz

================================================================================
来源：http://ycd.yj202588.top

H. 异常与错误处理
来源：http://ftu.shzxlz.cn

================================================================================
来源：http://jfg.ybcxt.top

[H01] try / catch 基础
来源：http://bxv.zhijiandao.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://phm.gaohongyu789.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ogy.zdqjudy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nce.xylfe.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xgw.hongshengwenyu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rkk.zhiwuduotai.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wfs.xziqi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zbx.pycfn.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xat.yonumen.top

[H02] finally / ensure 收尾
来源：http://isf.zhongyouzk.top

Py:   try: f()⏎finally: cleanup()
来源：http://hjx.pengpengdd.cyou

PHP:  try { f(); } finally { cleanup(); }
来源：http://lrp.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lyk.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nzu.yonumen.top

Java: try { f(); } finally { cleanup(); }
来源：http://vzv.tianlin.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://mzb.fanxiaobao.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://uyu.zycfv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jtt.bbcook.cn

[H03] 主动抛出异常
来源：http://gfi.sufxvd.cn

Py:   raise ValueError("错误信息")
来源：http://qva.chenlongwang.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dtn.hfpthk.cn

JS:   throw new Error("错误信息");
来源：http://fhr.ehwqpu.com

TS:   throw new Error("错误信息");
来源：http://adi.hesvh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nem.hongshengwenyu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://akz.nanxinkj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://heq.nwbrower.top

C#:   throw new ArgumentException("错误信息");
来源：http://yig.jinqigufen.top

[H04] 自定义异常类型
来源：http://jvr.yj20258888.top

Py:   class MyError(Exception): pass
来源：http://ufe.jyoumei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rgj.jlsjyb.cn

JS:   class MyError extends Error {}
来源：http://euc.jqgufenzy.top

TS:   class MyError extends Error {}
来源：http://tbg.daxiang520.top

Java: class MyException extends RuntimeException {}
来源：http://lvh.zhongyouzk.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yxx.jinqigufen.top

Ruby: class MyError < StandardError; end
来源：http://anv.bjfxy.top

C#:   class MyException : Exception {}
来源：http://wrl.cheryme.top

[H05] 捕获特定类型
来源：http://uvm.sxryk.cn

Py:   except ValueError as e:
来源：http://ibs.zhoulong.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yqk.sjlbkw.cn

JS:   if (e instanceof TypeError) {}
来源：http://csw.shanyushiyangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://ava.meibo888.top

Java: catch (IOException | SQLException e) {}
来源：http://hfg.wangdashe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fsp.ehwqpu.com

Ruby: rescue ArgumentError => e
来源：http://kdk.xziqi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lqz.yuanzhike.top

[H06] 可选值 / 空值安全访问
来源：http://fph.wangshuangyany.cn

Py:   value = d.get("k") or default
来源：http://nht.yanxiufei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lws.chenzaomai.com

JS:   obj?.a?.b;  d ?? default
来源：http://gld.iojbl.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kmv.jianghu66.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iay.shangyingyoupin.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xzb.yuanzhike.top

Ruby: d&.dig(:a, :b)
来源：http://rbj.kuanghao11.cn

C#:   obj?.A?.B ?? default
来源：http://zva.zhixingplan.top

[H07] 断言
来源：http://kty.chenjidiqi.icu

Py:   assert x > 0, "必须为正"
来源：http://csi.xziqi.cn

PHP:  assert($x > 0);
来源：http://osu.vehdjk.com

JS:   console.assert(x > 0);
来源：http://xim.fktsv.cn

TS:   console.assert(x > 0);
来源：http://efp.aizwys.cn

Java: assert x > 0 : "必须为正";
来源：http://yjr.quarkkingdee.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xhv.gogol.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ryi.tarul.cn

C#:   Debug.Assert(x > 0);
来源：http://cvt.cucudq.cn

[H08] 获取错误信息与堆栈
来源：http://zzk.hammf.cn

Py:   str(e);  traceback.format_exc()
来源：http://ala.daxiang520.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kyp.aibaodan.cn

JS:   e.message;  e.stack
来源：http://nwv.zhaomingkeji.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://gbx.chenlongwang.top

Java: e.getMessage();  e.printStackTrace()
来源：http://moa.dianchejie.cn

Go:   err.Error()
来源：http://ljh.ivvv.top

Ruby: e.message;  e.backtrace
来源：http://hry.ppjwa.cn

C#:   e.Message;  e.StackTrace
来源：http://hta.jlsjyb.cn

[H09] 带错误码的异常
来源：http://xyt.zhiwuduotai.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://syy.hywenlv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rzr.jqgufenzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fzf.pengpengdd.cyou

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pht.zhaomingkeji.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mvs.uphjek.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lfi.cdnleiting.top

Ruby: raise MyError.new("fail", 500)
来源：http://viq.cashguo.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qgh.c1oappe.top

[H10] 资源自动释放
来源：http://ieo.cdnleiting.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qaq.cucudq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fmq.chenzaomai.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jqj.iojbl.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gut.zhengqikj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nod.xziqi.cn

Go:   defer f.Close()
来源：http://xvp.jiagoushi.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uhi.gaohongyu789.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ked.daria6918.cn

================================================================================
来源：http://ucz.hammf.cn

I. 正则表达式
来源：http://bps.9152youxi.cn

================================================================================
来源：http://ptu.zhijiandao.cn

[I01] 判断是否匹配
来源：http://pga.bbcook.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://elj.chenzaomai.com

PHP:  preg_match('/\d+/', $s);
来源：http://qju.kuanghao11.cn

JS:   /\d+/.test(s)
来源：http://vdv.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://akf.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kul.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nqi.zdqjudy.top

Ruby: s.match?(/\d+/)
来源：http://ztw.jinghuilouyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://but.xuetiantiany.cn

[I02] 提取所有匹配
来源：http://cjj.chenjidiqi.icu

Py:   re.findall(r"\d+", s)
来源：http://upz.ivvv.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://whw.yanxiufei.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pyd.316326.xyz

TS:   s.match(/\d+/g)
来源：http://elp.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://axw.zycfv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ods.yongpay.top

Ruby: s.scan(/\d+/)
来源：http://ste.ppjwa.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bfq.52xcode.cn

[I03] 提取捕获分组
来源：http://dyz.tanke756.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jmc.chenlongwang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zmr.nanxuanxn.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cat.9152youxi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bpo.jianghu66.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wuf.jinghuilouyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uik.chenjidiqi.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://miq.xingfuxueyuan.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tiq.redwolf501.top

[I04] 正则替换
来源：http://dnt.sysykeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fbv.gzhubu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gil.mhx1999.top

JS:   s.replace(/\d+/g, "#")
来源：http://bxr.smart0.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://omy.mhx1999.top

Java: s.replaceAll("\\d+", "#")
来源：http://amz.hammf.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://igk.zhengqikj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nyh.ybcxt.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jqt.sufxvd.cn

[I05] 按正则拆分
来源：http://yud.havefunace.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wqp.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jwr.bbcook.cn

JS:   s.split(/\s*,\s*/)
来源：http://ett.yj20258888.top

TS:   s.split(/\s*,\s*/)
来源：http://egn.c1oappe.top

Java: s.split("\\s*,\\s*")
来源：http://tui.vqdsnc.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wat.fzhhl.top

Ruby: s.split(/\s*,\s*/)
来源：http://bhm.ivvv.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qss.chenjidiqi.icu

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gnq.jinqigfzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vuv.jinqigufen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bdm.yueranfly.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tcj.yj202588.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cpc.wangdashe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uxt.cashguo.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vsq.9152youxi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zrz.sxryk.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fvk.ivvv.top

[I07] 忽略大小写与多行模式
来源：http://tby.svipenyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gat.zycfv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sya.guannengcc.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://flk.xingfuxueyuan.xyz

TS:   /error/gim
来源：http://oqg.bbcook.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gtv.aibaodan.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ljo.cucudq.cn

Ruby: s.scan(/error/i)
来源：http://dxf.hongshengwenyu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jgg.ydjk.org.cn

[I08] 贪婪与非贪婪匹配
来源：http://hjv.snrcjt.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ykr.hesvh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fhw.gogol.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iqg.jyoumei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kdn.52xcode.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hsf.yonumen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xdh.nwbrower.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qql.zdbjq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dww.jiagoushi.top

================================================================================
来源：http://aaw.meibo888.top

J. 日期与时间
来源：http://jbd.zhijiandao.cn

================================================================================
来源：http://fbz.xuanzx.com

[J01] 获取当前时间
来源：http://enr.pengpengdd.cyou

Py:   datetime.now();  datetime.now(UTC)
来源：http://ihy.hfpthk.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ccd.chenlongwang.top

JS:   new Date();  Date.now()
来源：http://pwp.epnwcf.com

TS:   new Date();  Date.now()
来源：http://qlt.zycfv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fjq.guannengcc.top

Go:   time.Now()
来源：http://geb.jinqigfzy.top

Ruby: Time.now
来源：http://rpy.jinqigfzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nfp.jqgfzy.top

[J02] 格式化输出
来源：http://cau.zdbjq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://std.0kj1m.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dxq.daria6918.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://luc.cqqwz.cn

TS:   d.toISOString()
来源：http://dwt.shanyushiyangkeji.top


<!-- 参考信息 -->