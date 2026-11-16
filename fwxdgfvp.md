代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://pmi.wangdashe.top

Java: @Override String greet() { return "admin"; }
来源：http://btg.gotoacloud.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vxl.bbcook.cn

Ruby: def greet; "admin"; end
来源：http://rjv.yj202588.top

C#:   public override string Greet() => "admin";
来源：http://lpw.gotoacloud.top

[G07] 调用父类方法
来源：http://lqp.gogol.net.cn

Py:   super().greet()
来源：http://lwl.gaohongyu789.top

PHP:  parent::greet();
来源：http://ppk.sxryk.cn

JS:   super.greet();
来源：http://wcm.0kj1m.cn

TS:   super.greet();
来源：http://rie.gotoacloud.top

Java: super.greet();
来源：http://krb.cashguo.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fce.tian-w.cn

Ruby: super
来源：http://rzb.yj20258.top

C#:   base.Greet();
来源：http://imh.wangdashe.top

[G08] 静态方法与属性
来源：http://zlt.hnqzz.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lgh.fanxiaobao.xyz

PHP:  public static function f() {}
来源：http://jpy.cqqwz.cn

JS:   static f() {}
来源：http://lag.vehdjk.com

TS:   static f(): void {}
来源：http://tkq.nwbrower.top

Java: static void f() {}
来源：http://pmt.cdnleiting.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://lbg.snrcjt.cn

Ruby: def self.f; end
来源：http://hdz.zhengqikj.top

C#:   public static void F() {}
来源：http://tio.shangyingyoupin.top

[G09] 接口 / 抽象类
来源：http://rqw.zhoulong.xyz

Py:   from abc import ABC, abstractmethod
来源：http://ild.tian-w.cn

PHP:  interface Shape { public function area(): float; }
来源：http://akx.zdbjq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://osp.jyoumei.cn

TS:   interface Shape { area(): number; }
来源：http://rkp.aibaodan.cn

Java: interface Shape { double area(); }
来源：http://ngd.dianchejie.cn

Go:   type Shape interface { Area() float64 }
来源：http://vga.vehdjk.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mio.zhaomingkeji.xyz

C#:   interface IShape { double Area(); }
来源：http://izg.jinqigufen.top

[G10] 访问控制
来源：http://sog.jianghu66.top

Py:   约定 _protected / __private（不强制）
来源：http://vwf.aibaodan.cn

PHP:  public / protected / private
来源：http://bdm.zhaomingkeji.xyz

JS:   #private 字段；其余公开
来源：http://hci.xziqi.cn

TS:   public / protected / private
来源：http://cxe.zdqjudy.top

Java: public / protected / private / 默认包级
来源：http://eki.kuanghao11.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xfc.cqqwz.cn

Ruby: public / protected / private
来源：http://jjf.xylfe.cn

C#:   public / protected / private / internal
来源：http://vjq.zdqjudy.top

[G11] getter / setter
来源：http://fjn.tanke756.top

Py:   @property 与 @x.setter
来源：http://ord.vqdsnc.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://srv.sxryk.cn

JS:   get name() { return this._name; }
来源：http://vqd.sysykeji.top

TS:   get name(): string { return this._name; }
来源：http://uhe.vehdjk.com

Java: public String getName() { return name; }
来源：http://eqf.zhaomingkeji.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://qqo.vehdjk.com

Ruby: attr_accessor :name
来源：http://icr.jqgfzy.top

C#:   public string Name { get; set; }
来源：http://hfh.mhx1999.top

[G12] 对象转字符串
来源：http://yhv.jinqigfzy.top

Py:   def __str__(self): return self.name
来源：http://tzt.ydzc1.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rtr.hesvh.cn

JS:   toString() { return this.name; }
来源：http://ddg.havefunace.top

TS:   toString(): string { return this.name; }
来源：http://bcc.feifeiyinyue.top

Java: @Override public String toString() { return name; }
来源：http://vry.jinghuilouyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tzw.jinqigfzy.top

Ruby: def to_s; @name; end
来源：http://czj.hcnkem.com

C#:   public override string ToString() => Name;
来源：http://hxn.feifeiyinyue.top

[G13] 判断对象类型
来源：http://qnz.jyoumei.cn

Py:   isinstance(u, User)
来源：http://khv.ivvv.top

PHP:  $u instanceof User
来源：http://qtt.jiagoushi.top

JS:   u instanceof User
来源：http://mxd.cdnleiting.top

TS:   u instanceof User
来源：http://igt.sxryk.cn

Java: u instanceof User
来源：http://dvk.chenjidiqi.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://glt.cheryme.top

Ruby: u.is_a?(User)
来源：http://ont.yueranfly.top

C#:   u is User
来源：http://jsu.hongshengwenyu.top

[G14] 数据类 / record
来源：http://yik.mhx1999.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://eub.jlsjyb.cn

PHP:  // 用 readonly 属性模拟
来源：http://pqi.ppjwa.cn

JS:   // 无内置：普通类或对象字面量
来源：http://iqp.wangdashe.top

TS:   type User = { name: string; age: number };
来源：http://xkl.nanxinkj.top

Java: record User(String name, int age) {}
来源：http://ida.aibaodan.cn

Go:   type User struct { Name string; Age int }
来源：http://bym.tanke756.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ngx.quarkkingdee.top

C#:   record User(string Name, int Age);
来源：http://sef.jyoumei.cn

[G15] 枚举
来源：http://eeq.52xcode.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kim.shzxlz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pwc.zdqjudy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cfa.shuidangran.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nfx.epnwcf.com

Java: enum Color { RED, GREEN }
来源：http://dsx.tarul.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qza.bbcook.cn

Ruby: Color = %i[red green].freeze
来源：http://jac.jlsjyb.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fdj.zhijiandao.cn

[G16] 对象转数组 / 字典
来源：http://tjy.nanxuanxn.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eim.chenjidiqi.icu

PHP:  get_object_vars($obj);
来源：http://unb.zhoulong.xyz

JS:   Object.entries(obj)
来源：http://rgw.tianlin.xyz

TS:   Object.entries(obj)
来源：http://ayk.shanyushiyangtech.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://eqg.guannengcc.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gvy.gotoacloud.top

Ruby: obj.instance_variables
来源：http://bxr.jqgufenzy.top

C#:   // 用反射或 System.Text.Json
来源：http://eha.ydzc1.top

================================================================================
来源：http://inl.yj20258.top

H. 异常与错误处理
来源：http://xet.yj20258.top

================================================================================
来源：http://lga.hywenlv.cn

[H01] try / catch 基础
来源：http://fxl.daxiang520.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://feu.jinqigfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rcr.9152youxi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vzm.fzhhl.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jth.vehdjk.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tre.tian-w.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yac.aizwys.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gnf.havefunace.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rlr.nwbrower.top

[H02] finally / ensure 收尾
来源：http://lrr.hongshengwenyu.top

Py:   try: f()⏎finally: cleanup()
来源：http://mpv.dianchejie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qrk.cqqwz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ibn.yfazqb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://cbt.hammf.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uzt.haohaochexian.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://qns.hammf.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jkh.xziqi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tgo.yangfankeji.com

[H03] 主动抛出异常
来源：http://xvt.sweek.top

Py:   raise ValueError("错误信息")
来源：http://baz.yj20258888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://knh.zdbjq.cn

JS:   throw new Error("错误信息");
来源：http://gje.gogol.net.cn

TS:   throw new Error("错误信息");
来源：http://eab.sysykeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rmc.yfazqb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wll.quarkkingdee.top

Ruby: raise ArgumentError, "错误信息"
来源：http://wax.zdqjudy.top

C#:   throw new ArgumentException("错误信息");
来源：http://bdv.sxryk.cn

[H04] 自定义异常类型
来源：http://vht.yfazqb.com

Py:   class MyError(Exception): pass
来源：http://ztu.jinqigufen.top

PHP:  class MyError extends RuntimeException {}
来源：http://hqs.xuetiantiany.cn

JS:   class MyError extends Error {}
来源：http://nsd.hfpthk.cn

TS:   class MyError extends Error {}
来源：http://lpl.hesvh.cn

Java: class MyException extends RuntimeException {}
来源：http://pof.zhiwuduotai.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://anx.sxryk.cn

Ruby: class MyError < StandardError; end
来源：http://ywq.jiagoushi.top

C#:   class MyException : Exception {}
来源：http://vwd.sufxvd.cn

[H05] 捕获特定类型
来源：http://ukl.shanyushiyangkeji.top

Py:   except ValueError as e:
来源：http://jes.ivvv.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pyc.yj20258888.top

JS:   if (e instanceof TypeError) {}
来源：http://akz.zhiwuduotai.top

TS:   if (e instanceof TypeError) {}
来源：http://cpb.sjlbkw.cn

Java: catch (IOException | SQLException e) {}
来源：http://wkb.bbcook.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pqc.cheryme.top

Ruby: rescue ArgumentError => e
来源：http://ppp.tian-w.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ltk.aizwys.cn

[H06] 可选值 / 空值安全访问
来源：http://fng.dianchejie.cn

Py:   value = d.get("k") or default
来源：http://ext.zycfv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ibb.zhoulong.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://hdv.hysaishi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rhy.jqgufenzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qvo.ivvv.top

Go:   if v, ok := m["k"]; ok { }
来源：http://tge.hfpthk.cn

Ruby: d&.dig(:a, :b)
来源：http://hpv.ctjpmb.com

C#:   obj?.A?.B ?? default
来源：http://emb.xziqi.cn

[H07] 断言
来源：http://ppx.yj20258888.top

Py:   assert x > 0, "必须为正"
来源：http://egl.hammf.cn

PHP:  assert($x > 0);
来源：http://tzg.yuxming.cn

JS:   console.assert(x > 0);
来源：http://mdh.shanyushiyangtech.top

TS:   console.assert(x > 0);
来源：http://tby.sjlbkw.cn

Java: assert x > 0 : "必须为正";
来源：http://qib.xziqi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lxi.feifeiyinyue.top

Ruby: raise "必须为正" unless x > 0
来源：http://giy.yuxming.cn

C#:   Debug.Assert(x > 0);
来源：http://meg.ctjpmb.com

[H08] 获取错误信息与堆栈
来源：http://yja.ywan-chungtsiang.top

Py:   str(e);  traceback.format_exc()
来源：http://tlr.xingfuxueyuan.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fxc.nanxuanxn.top

JS:   e.message;  e.stack
来源：http://xeb.yj20258888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hrd.smart0.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://nar.redwolf501.top

Go:   err.Error()
来源：http://quz.cqqwz.cn

Ruby: e.message;  e.backtrace
来源：http://czr.smart0.xyz

C#:   e.Message;  e.StackTrace
来源：http://aei.aizwys.cn

[H09] 带错误码的异常
来源：http://xlc.zhiwuduotai.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jtr.nwbrower.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ota.vehdjk.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nze.jinyuanbaomall.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uah.fengsongda.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kur.shuidangran.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kzw.yj20258888.top

Ruby: raise MyError.new("fail", 500)
来源：http://tdj.feifeiyinyue.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pkf.xuanzx.com

[H10] 资源自动释放
来源：http://iha.tarul.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://voj.zhongyouzk.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gcn.aizwys.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bjd.jianghu66.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xsb.yuanzhike.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wsl.jiagoushi.top

Go:   defer f.Close()
来源：http://xll.feifeiyinyue.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wok.chenjidiqi.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rwz.shanyushiyangtech.top

================================================================================
来源：http://pdv.zdqjudy.top

I. 正则表达式
来源：http://kwz.jinqigfzy.top

================================================================================
来源：http://mzn.nanxuanxn.top

[I01] 判断是否匹配
来源：http://bmy.yueranfly.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zrm.yvedp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cbw.9152youxi.cn

JS:   /\d+/.test(s)
来源：http://inf.pycfn.com

TS:   /\d+/.test(s)
来源：http://sbd.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zuy.aizwys.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iaj.xuetiantiany.cn

Ruby: s.match?(/\d+/)
来源：http://kbh.daria6918.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rsv.aizwys.cn

[I02] 提取所有匹配
来源：http://ujn.yonumen.top

Py:   re.findall(r"\d+", s)
来源：http://lyt.bjfxy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://guh.gaohongyu789.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ieq.yongpay.top

TS:   s.match(/\d+/g)
来源：http://rtb.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dbq.birdmap.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mkp.dashuyun.cn

Ruby: s.scan(/\d+/)
来源：http://rdo.sysykeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://msm.haohaochexian.top

[I03] 提取捕获分组
来源：http://srw.yvedp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ikn.gzhubu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ttj.wangdashe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://enk.wangdashe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xzg.cdnleiting.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://czp.hnqzz.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pvv.chenjidiqi.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pup.9152youxi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ghx.tian-w.cn

[I04] 正则替换
来源：http://ezd.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ehj.jinyuanbaomall.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gns.xylfe.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bcj.ppjwa.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zfo.yuxming.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gtt.cheryme.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pnn.yvedp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uij.nwbrower.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uzr.ydjk.org.cn

[I05] 按正则拆分
来源：http://ult.zhiwuduotai.top

Py:   re.split(r"\s*,\s*", s)
来源：http://kve.meibo888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://orw.yuanzhike.top

JS:   s.split(/\s*,\s*/)
来源：http://jdr.gaohongyu789.top

TS:   s.split(/\s*,\s*/)
来源：http://xck.zycfv.cn

Java: s.split("\\s*,\\s*")
来源：http://bxo.gzhubu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lhf.vehdjk.com

Ruby: s.split(/\s*,\s*/)
来源：http://xtm.chenjidiqi.icu

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fwf.hcnkem.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qyf.jyoumei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wzf.c1oappe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dgv.bbcook.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mup.sufxvd.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kur.meibo888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vdw.chenlongwang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fot.meibo888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://iht.hysaishi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qmo.daria6918.cn

[I07] 忽略大小写与多行模式
来源：http://ehh.sweek.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pns.hongshengwenyu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://znv.yongpay.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lbp.dianchejie.cn

TS:   /error/gim
来源：http://hkm.uphjek.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://doq.jlsjyb.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kac.xylfe.cn

Ruby: s.scan(/error/i)
来源：http://dsr.ybcxt.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mat.jqgfzy.top

[I08] 贪婪与非贪婪匹配
来源：http://vcg.smart0.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zux.yj20258.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jdh.nanxinkj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://erg.jianghu66.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jtx.jqgfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ahy.xziqi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gst.jianghu66.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rmw.fengsongda.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rdr.zhiwuduotai.top

================================================================================
来源：http://xbq.zhongyouzk.top

J. 日期与时间
来源：http://bjc.0kj1m.cn

================================================================================
来源：http://lvo.tarul.cn

[J01] 获取当前时间
来源：http://chw.zhijiandao.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rmi.dashuyun.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yzt.guowangkeji.top

JS:   new Date();  Date.now()
来源：http://ofk.jinyuanbaomall.cn

TS:   new Date();  Date.now()
来源：http://tmf.guowangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://mvi.sweek.top

Go:   time.Now()
来源：http://lwu.zycfv.cn

Ruby: Time.now
来源：http://vtg.yueranfly.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ipq.c1oappe.top

[J02] 格式化输出
来源：http://xxp.xingfuxueyuan.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://erx.zhixingplan.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bfs.cashguo.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nkq.jyoumei.cn

TS:   d.toISOString()
来源：http://nio.hongshengwenyu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sls.gzhubu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://apx.xuanzx.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qfb.bjfxy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://myg.iojbl.cn

[J03] 字符串解析为日期
来源：http://cwz.jianghu66.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mca.jinqigfzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ors.fktsv.cn

JS:   new Date("2024-01-02")
来源：http://xyo.c1oappe.top

TS:   new Date("2024-01-02")
来源：http://opp.dianchejie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xrd.zhiwuduotai.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://weh.jianghu66.top

Ruby: Date.parse("2024-01-02")
来源：http://pjq.yueranfly.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lhl.yj20258888.top

[J04] 时间戳与日期互转
来源：http://rfy.havefunace.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xjz.nanxinkj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zoo.zycfv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ozm.havefunace.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ckr.sysykeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uet.daria6918.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fax.birdmap.top


<!-- 参考信息 -->