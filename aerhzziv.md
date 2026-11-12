代发 wailian999

[G06] 重写方法
来源：http://qrb.chenjidiqi.icu

Py:   def greet(self): return "admin"
来源：http://eyc.ydjk.org.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jcy.pengpengdd.cyou

JS:   greet() { return "admin"; }
来源：http://isa.sxryk.cn

TS:   greet(): string { return "admin"; }
来源：http://fof.cdnleiting.top

Java: @Override String greet() { return "admin"; }
来源：http://wlu.feifeiyinyue.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eti.daria6918.cn

Ruby: def greet; "admin"; end
来源：http://yxd.mhx1999.top

C#:   public override string Greet() => "admin";
来源：http://wjf.zhongyouzk.top

[G07] 调用父类方法
来源：http://hxw.cqqwz.cn

Py:   super().greet()
来源：http://las.zhaomingkeji.xyz

PHP:  parent::greet();
来源：http://mse.zycfv.cn

JS:   super.greet();
来源：http://cbe.redwolf501.top

TS:   super.greet();
来源：http://xfb.wangshuangyany.cn

Java: super.greet();
来源：http://bxh.hesvh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://isc.wangshuangyany.cn

Ruby: super
来源：http://jgo.tarul.cn

C#:   base.Greet();
来源：http://iec.aibaodan.cn

[G08] 静态方法与属性
来源：http://tcl.haohaochexian.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://csg.snrcjt.cn

PHP:  public static function f() {}
来源：http://iwl.hongshengwenyu.top

JS:   static f() {}
来源：http://vts.zdqjudy.top

TS:   static f(): void {}
来源：http://iyh.jinghuilouyu.cn

Java: static void f() {}
来源：http://yeq.zhixingplan.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ury.yanxiufei.cn

Ruby: def self.f; end
来源：http://mad.yangfankeji.com

C#:   public static void F() {}
来源：http://ugb.uphjek.com

[G09] 接口 / 抽象类
来源：http://sov.uphjek.com

Py:   from abc import ABC, abstractmethod
来源：http://bxq.vqdsnc.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rgr.yuanzhike.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://dja.sufxvd.cn

TS:   interface Shape { area(): number; }
来源：http://kca.kuanghao11.cn

Java: interface Shape { double area(); }
来源：http://bur.fengsongda.top

Go:   type Shape interface { Area() float64 }
来源：http://yml.yuanzhike.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ucv.yangfankeji.com

C#:   interface IShape { double Area(); }
来源：http://gtc.nwbrower.top

[G10] 访问控制
来源：http://eas.uphjek.com

Py:   约定 _protected / __private（不强制）
来源：http://dnt.tanke756.top

PHP:  public / protected / private
来源：http://wfz.shangyingyoupin.top

JS:   #private 字段；其余公开
来源：http://qim.gzhubu.top

TS:   public / protected / private
来源：http://gvp.nwbrower.top

Java: public / protected / private / 默认包级
来源：http://ulo.yueranfly.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zmc.tian-w.cn

Ruby: public / protected / private
来源：http://ynx.xingfuxueyuan.xyz

C#:   public / protected / private / internal
来源：http://ery.svipenyu.cn

[G11] getter / setter
来源：http://ddm.gzhubu.top

Py:   @property 与 @x.setter
来源：http://myh.zhoulong.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://teh.svipenyu.cn

JS:   get name() { return this._name; }
来源：http://ccb.mhx1999.top

TS:   get name(): string { return this._name; }
来源：http://ipe.snrcjt.cn

Java: public String getName() { return name; }
来源：http://gbe.andypj.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://wmy.bjfxy.top

Ruby: attr_accessor :name
来源：http://ftr.hnqzz.top

C#:   public string Name { get; set; }
来源：http://rua.fzhhl.top

[G12] 对象转字符串
来源：http://cth.52xcode.cn

Py:   def __str__(self): return self.name
来源：http://qpu.zhoulong.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://pgf.gaohongyu789.top

JS:   toString() { return this.name; }
来源：http://sin.ybcxt.top

TS:   toString(): string { return this.name; }
来源：http://kpm.yvedp.cn

Java: @Override public String toString() { return name; }
来源：http://qqp.yonumen.top

Go:   func (u User) String() string { return u.Name }
来源：http://hiv.jyoumei.cn

Ruby: def to_s; @name; end
来源：http://trt.hammf.cn

C#:   public override string ToString() => Name;
来源：http://jfy.9152youxi.cn

[G13] 判断对象类型
来源：http://nxq.ybcxt.top

Py:   isinstance(u, User)
来源：http://hqv.fengsongda.top

PHP:  $u instanceof User
来源：http://sow.yanxiufei.cn

JS:   u instanceof User
来源：http://rar.zhengqikj.top

TS:   u instanceof User
来源：http://izn.yj20258888.top

Java: u instanceof User
来源：http://pdq.yueranfly.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kbt.0kj1m.cn

Ruby: u.is_a?(User)
来源：http://sgp.ydzc1.top

C#:   u is User
来源：http://whm.xuanzx.com

[G14] 数据类 / record
来源：http://htp.daria6918.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mfv.epnwcf.com

PHP:  // 用 readonly 属性模拟
来源：http://asn.bjfxy.top

JS:   // 无内置：普通类或对象字面量
来源：http://rbb.dianchejie.cn

TS:   type User = { name: string; age: number };
来源：http://pqi.yuxming.cn

Java: record User(String name, int age) {}
来源：http://yhq.zhengqikj.top

Go:   type User struct { Name string; Age int }
来源：http://kwx.zhixingplan.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ozy.jinqigufen.top

C#:   record User(string Name, int Age);
来源：http://odl.shangyingyoupin.top

[G15] 枚举
来源：http://flt.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://voq.bbcook.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xes.smart0.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zap.ivvv.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hlx.svipenyu.cn

Java: enum Color { RED, GREEN }
来源：http://awc.cqqwz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pmg.sysykeji.top

Ruby: Color = %i[red green].freeze
来源：http://nxy.kuanghao11.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://aij.vehdjk.com

[G16] 对象转数组 / 字典
来源：http://tpb.zdqjudy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iur.jinyuanbaomall.cn

PHP:  get_object_vars($obj);
来源：http://dqu.yongpay.top

JS:   Object.entries(obj)
来源：http://foj.zdqjudy.top

TS:   Object.entries(obj)
来源：http://yqg.yj20258888.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vlk.chenzaomai.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://ytt.ivvv.top

Ruby: obj.instance_variables
来源：http://sbj.aibaodan.cn

C#:   // 用反射或 System.Text.Json
来源：http://vax.sweek.top

================================================================================
来源：http://apk.haohaochexian.top

H. 异常与错误处理
来源：http://cxn.zdqjudy.top

================================================================================
来源：http://wtw.guowangkeji.top

[H01] try / catch 基础
来源：http://vly.ctjpmb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nsz.jinghuilouyu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ixb.52xcode.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tlw.sxryk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yhy.gzhubu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mmp.vehdjk.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zjt.nanxinkj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zup.hongshengwenyu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jri.cheryme.top

[H02] finally / ensure 收尾
来源：http://jvj.xinyue.icu

Py:   try: f()⏎finally: cleanup()
来源：http://kyl.fengsongda.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://our.smart0.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://tfa.zhixingplan.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zhr.cashguo.top

Java: try { f(); } finally { cleanup(); }
来源：http://bbz.zhengqikj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hzj.pycfn.com

Ruby: begin; f; ensure; cleanup; end
来源：http://eut.xuanzx.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://djf.dianchejie.cn

[H03] 主动抛出异常
来源：http://kqv.kuanghao11.cn

Py:   raise ValueError("错误信息")
来源：http://tpf.zhiwuduotai.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hxk.jyoumei.cn

JS:   throw new Error("错误信息");
来源：http://bjl.jqgfzy.top

TS:   throw new Error("错误信息");
来源：http://fyw.ydzc1.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rpk.jlsjyb.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qem.xinyue.icu

Ruby: raise ArgumentError, "错误信息"
来源：http://zsl.ybcxt.top

C#:   throw new ArgumentException("错误信息");
来源：http://gio.sjlbkw.cn

[H04] 自定义异常类型
来源：http://vfv.meibo888.top

Py:   class MyError(Exception): pass
来源：http://hah.haohaochexian.top

PHP:  class MyError extends RuntimeException {}
来源：http://clq.gogol.net.cn

JS:   class MyError extends Error {}
来源：http://nnh.xingfuxueyuan.xyz

TS:   class MyError extends Error {}
来源：http://qcj.xuanzx.com

Java: class MyException extends RuntimeException {}
来源：http://atp.xinyue.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vls.ywan-chungtsiang.top

Ruby: class MyError < StandardError; end
来源：http://bky.wangshuangyany.cn

C#:   class MyException : Exception {}
来源：http://xyl.ppjwa.cn

[H05] 捕获特定类型
来源：http://evb.gotoacloud.top

Py:   except ValueError as e:
来源：http://dtj.gzhubu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lin.vehdjk.com

JS:   if (e instanceof TypeError) {}
来源：http://sta.yj20258888.top

TS:   if (e instanceof TypeError) {}
来源：http://ayf.zhixingplan.top

Java: catch (IOException | SQLException e) {}
来源：http://tsr.chenlongwang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qrq.pycfn.com

Ruby: rescue ArgumentError => e
来源：http://vrz.vqdsnc.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gmq.jianghu66.top

[H06] 可选值 / 空值安全访问
来源：http://tjs.quarkkingdee.top

Py:   value = d.get("k") or default
来源：http://ciy.haohaochexian.top

PHP:  $v = $d["k"] ?? null;
来源：http://gss.jqgufenzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://vfy.aizwys.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uin.fktsv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sjg.epnwcf.com

Go:   if v, ok := m["k"]; ok { }
来源：http://ifb.epnwcf.com

Ruby: d&.dig(:a, :b)
来源：http://vwt.0kj1m.cn

C#:   obj?.A?.B ?? default
来源：http://gmb.yfazqb.com

[H07] 断言
来源：http://upj.yuanzhike.top

Py:   assert x > 0, "必须为正"
来源：http://tiu.hnxiangtu.top

PHP:  assert($x > 0);
来源：http://mzq.ywan-chungtsiang.top

JS:   console.assert(x > 0);
来源：http://ewi.shzxlz.cn

TS:   console.assert(x > 0);
来源：http://wod.shzxlz.cn

Java: assert x > 0 : "必须为正";
来源：http://ulg.ydjk.org.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ckl.jianghu66.top

Ruby: raise "必须为正" unless x > 0
来源：http://hxv.aibaodan.cn

C#:   Debug.Assert(x > 0);
来源：http://ecg.cheryme.top

[H08] 获取错误信息与堆栈
来源：http://uqj.yj202588.top

Py:   str(e);  traceback.format_exc()
来源：http://vkr.havefunace.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zkx.tanke756.top

JS:   e.message;  e.stack
来源：http://qen.52xcode.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sza.sjlbkw.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wez.mhx1999.top

Go:   err.Error()
来源：http://ooo.nwbrower.top

Ruby: e.message;  e.backtrace
来源：http://ufj.wangshuangyany.cn

C#:   e.Message;  e.StackTrace
来源：http://uyb.ywan-chungtsiang.top

[H09] 带错误码的异常
来源：http://wsa.chenlongwang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wtj.guowangkeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://nwr.yfazqb.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yya.hammf.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lir.sjlbkw.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hdp.ydjk.org.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://map.guowangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://hpc.snrcjt.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hdm.zhijiandao.cn

[H10] 资源自动释放
来源：http://pxj.zhongyouzk.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vdh.yfazqb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dmf.shuidangran.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://avw.nanxuanxn.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://evg.shanyushiyangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://out.tian-w.cn

Go:   defer f.Close()
来源：http://jun.ctjpmb.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fgr.ehwqpu.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cut.yongpay.top

================================================================================
来源：http://wgi.zhoulong.xyz

I. 正则表达式
来源：http://nfb.snrcjt.cn

================================================================================
来源：http://qyt.jqgfzy.top

[I01] 判断是否匹配
来源：http://cjn.0kj1m.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cnf.hcnkem.com

PHP:  preg_match('/\d+/', $s);
来源：http://aup.tian-w.cn

JS:   /\d+/.test(s)
来源：http://yzy.xylfe.cn

TS:   /\d+/.test(s)
来源：http://aih.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vhw.kuanghao11.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vtt.hnqzz.top

Ruby: s.match?(/\d+/)
来源：http://jto.fehbvm.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://atr.yj202588.top

[I02] 提取所有匹配
来源：http://fbr.sufxvd.cn

Py:   re.findall(r"\d+", s)
来源：http://cuz.dianchejie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zsh.shanyushiyangkeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cda.quarkkingdee.top

TS:   s.match(/\d+/g)
来源：http://gcu.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kwt.yuxming.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qup.ydjk.org.cn

Ruby: s.scan(/\d+/)
来源：http://cbz.tanke756.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qxw.tarul.cn

[I03] 提取捕获分组
来源：http://dpb.gaohongyu789.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vtu.nanxinkj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mdg.yuanzhike.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nks.yongpay.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lrq.vqdsnc.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hix.hfpthk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tdr.vehdjk.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qhv.hysaishi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://asg.fengsongda.top

[I04] 正则替换
来源：http://nli.316326.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://tiu.zdqjudy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cem.yangfankeji.com

JS:   s.replace(/\d+/g, "#")
来源：http://qag.jinghuilouyu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lel.yueranfly.top

Java: s.replaceAll("\\d+", "#")
来源：http://xar.shanyushiyangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://gbo.nanxinkj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ymc.hnxiangtu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gsc.fengsongda.top

[I05] 按正则拆分
来源：http://rti.yj20258888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://noe.cucudq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bey.hysaishi.cn

JS:   s.split(/\s*,\s*/)
来源：http://hmk.redwolf501.top

TS:   s.split(/\s*,\s*/)
来源：http://myp.nanxuanxn.top

Java: s.split("\\s*,\\s*")
来源：http://law.bjfxy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://owr.iojbl.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pcp.yangfankeji.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hgl.shanyushiyangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jct.dashuyun.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jqs.tianlin.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rtn.zhiwuduotai.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dgv.yj202588.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dmh.ydjk.org.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cqa.snrcjt.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dsm.redwolf501.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ari.snrcjt.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zrv.ctjpmb.com

[I07] 忽略大小写与多行模式
来源：http://hzq.bjfxy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dcf.nanxuanxn.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tso.wangshuangyany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iax.yueranfly.top

TS:   /error/gim
来源：http://srv.nanxuanxn.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hav.ywan-chungtsiang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oxz.ehwqpu.com

Ruby: s.scan(/error/i)
来源：http://hbl.gogol.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fyh.yueranfly.top

[I08] 贪婪与非贪婪匹配
来源：http://vak.pengpengdd.cyou

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xgq.zdqjudy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gxz.jinghuilouyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hil.daxiang520.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://htr.yongpay.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qbw.dashuyun.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cju.yonumen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kuv.cucudq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fgv.jianghu66.top

================================================================================
来源：http://ndh.birdmap.top

J. 日期与时间
来源：http://bfe.quarkkingdee.top

================================================================================
来源：http://nui.daria6918.cn

[J01] 获取当前时间
来源：http://yyk.yuxming.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kes.yfazqb.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dlk.redwolf501.top

JS:   new Date();  Date.now()
来源：http://ntm.hysaishi.cn

TS:   new Date();  Date.now()
来源：http://nuk.zhaomingkeji.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://snb.bbcook.cn

Go:   time.Now()
来源：http://ppj.c1oappe.top

Ruby: Time.now
来源：http://vto.jyoumei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ith.yuanzhike.top

[J02] 格式化输出
来源：http://nud.sxryk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hlb.guowangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://smy.cucudq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://joc.zdbjq.cn

TS:   d.toISOString()
来源：http://vxy.shanyushiyangtech.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lia.andypj.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cja.redwolf501.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://krp.fanxiaobao.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fqx.fengsongda.top

[J03] 字符串解析为日期
来源：http://lbo.tanke756.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pyn.zycfv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fhb.nwbrower.top

JS:   new Date("2024-01-02")
来源：http://yqj.xingfuxueyuan.xyz

TS:   new Date("2024-01-02")
来源：http://vqw.gaohongyu789.top

Java: LocalDate.parse("2024-01-02")
来源：http://nku.gaohongyu789.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ebw.ywan-chungtsiang.top

Ruby: Date.parse("2024-01-02")
来源：http://sax.shanyushiyangtech.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ewg.shanyushiyangtech.top

[J04] 时间戳与日期互转
来源：http://bgq.tarul.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ypc.tanke756.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://udk.jinyuanbaomall.cn


<!-- 参考信息 -->