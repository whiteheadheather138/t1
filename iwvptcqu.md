代发 wailian999

[G06] 重写方法
来源：http://nwq.bjfxy.top

Py:   def greet(self): return "admin"
来源：http://cvy.316326.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://maq.kuanghao11.cn

JS:   greet() { return "admin"; }
来源：http://ggy.pycfn.com

TS:   greet(): string { return "admin"; }
来源：http://daq.hnxiangtu.top

Java: @Override String greet() { return "admin"; }
来源：http://gwc.cucudq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dbx.quarkkingdee.top

Ruby: def greet; "admin"; end
来源：http://qea.dianchejie.cn

C#:   public override string Greet() => "admin";
来源：http://enm.hnxiangtu.top

[G07] 调用父类方法
来源：http://lgq.xinyue.icu

Py:   super().greet()
来源：http://mhl.hnxiangtu.top

PHP:  parent::greet();
来源：http://qyv.hesvh.cn

JS:   super.greet();
来源：http://ple.zhaomingkeji.xyz

TS:   super.greet();
来源：http://syw.jlsjyb.cn

Java: super.greet();
来源：http://xnv.yangfankeji.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cpm.fengsongda.top

Ruby: super
来源：http://rmd.birdmap.top

C#:   base.Greet();
来源：http://nsh.fanxiaobao.xyz

[G08] 静态方法与属性
来源：http://cjq.svipenyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dpm.xylfe.cn

PHP:  public static function f() {}
来源：http://ltr.chenlongwang.top

JS:   static f() {}
来源：http://ecm.yueranfly.top

TS:   static f(): void {}
来源：http://nyv.pycfn.com

Java: static void f() {}
来源：http://sjw.xylfe.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pgn.shanyushiyangtech.top

Ruby: def self.f; end
来源：http://wld.redwolf501.top

C#:   public static void F() {}
来源：http://psr.zycfv.cn

[G09] 接口 / 抽象类
来源：http://mih.zhaomingkeji.xyz

Py:   from abc import ABC, abstractmethod
来源：http://arg.sufxvd.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yda.daxiang520.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xhz.xuetiantiany.cn

TS:   interface Shape { area(): number; }
来源：http://uaf.cheryme.top

Java: interface Shape { double area(); }
来源：http://ubf.fanxiaobao.xyz

Go:   type Shape interface { Area() float64 }
来源：http://per.jyoumei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wva.xziqi.cn

C#:   interface IShape { double Area(); }
来源：http://nfb.birdmap.top

[G10] 访问控制
来源：http://pdc.ppjwa.cn

Py:   约定 _protected / __private（不强制）
来源：http://sok.zhongyouzk.top

PHP:  public / protected / private
来源：http://ayg.aibaodan.cn

JS:   #private 字段；其余公开
来源：http://muh.chenzaomai.com

TS:   public / protected / private
来源：http://ssc.316326.xyz

Java: public / protected / private / 默认包级
来源：http://sks.yueranfly.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://krl.wangshuangyany.cn

Ruby: public / protected / private
来源：http://wpg.316326.xyz

C#:   public / protected / private / internal
来源：http://qxx.jinghuilouyu.cn

[G11] getter / setter
来源：http://ovx.bbcook.cn

Py:   @property 与 @x.setter
来源：http://iow.yueranfly.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bkw.vqdsnc.cn

JS:   get name() { return this._name; }
来源：http://mif.hfpthk.cn

TS:   get name(): string { return this._name; }
来源：http://vkz.hcnkem.com

Java: public String getName() { return name; }
来源：http://mdr.bbcook.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xtw.ybcxt.top

Ruby: attr_accessor :name
来源：http://iit.xuetiantiany.cn

C#:   public string Name { get; set; }
来源：http://yfv.yanxiufei.cn

[G12] 对象转字符串
来源：http://iyj.smart0.xyz

Py:   def __str__(self): return self.name
来源：http://dgt.ppjwa.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ngl.gogol.net.cn

JS:   toString() { return this.name; }
来源：http://ocq.shanyushiyangkeji.top

TS:   toString(): string { return this.name; }
来源：http://ocn.snrcjt.cn

Java: @Override public String toString() { return name; }
来源：http://ssc.guannengcc.top

Go:   func (u User) String() string { return u.Name }
来源：http://npn.cdnleiting.top

Ruby: def to_s; @name; end
来源：http://kyg.yueranfly.top

C#:   public override string ToString() => Name;
来源：http://lpa.jyoumei.cn

[G13] 判断对象类型
来源：http://dmw.sweek.top

Py:   isinstance(u, User)
来源：http://gbb.yfazqb.com

PHP:  $u instanceof User
来源：http://bnl.tian-w.cn

JS:   u instanceof User
来源：http://ynp.tian-w.cn

TS:   u instanceof User
来源：http://tak.redwolf501.top

Java: u instanceof User
来源：http://byn.dianchejie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zbn.jinqigfzy.top

Ruby: u.is_a?(User)
来源：http://xbn.nwbrower.top

C#:   u is User
来源：http://tks.guannengcc.top

[G14] 数据类 / record
来源：http://kyx.yj202588.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://npy.redwolf501.top

PHP:  // 用 readonly 属性模拟
来源：http://ejl.birdmap.top

JS:   // 无内置：普通类或对象字面量
来源：http://csv.guannengcc.top

TS:   type User = { name: string; age: number };
来源：http://piy.ehwqpu.com

Java: record User(String name, int age) {}
来源：http://tdw.gaohongyu789.top

Go:   type User struct { Name string; Age int }
来源：http://fmm.c1oappe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://few.c1oappe.top

C#:   record User(string Name, int Age);
来源：http://lnv.ivvv.top

[G15] 枚举
来源：http://fxc.yanxiufei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lts.jlsjyb.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://npz.wangshuangyany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oog.hnxiangtu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kbe.xinyue.icu

Java: enum Color { RED, GREEN }
来源：http://lrv.andypj.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uer.hesvh.cn

Ruby: Color = %i[red green].freeze
来源：http://ceq.jianghu66.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ani.uphjek.com

[G16] 对象转数组 / 字典
来源：http://rfs.0kj1m.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hjz.jqgfzy.top

PHP:  get_object_vars($obj);
来源：http://zhw.nanxinkj.top

JS:   Object.entries(obj)
来源：http://uzm.jqgfzy.top

TS:   Object.entries(obj)
来源：http://ezd.haohaochexian.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wfd.fzhhl.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tey.cheryme.top

Ruby: obj.instance_variables
来源：http://cls.aizwys.cn

C#:   // 用反射或 System.Text.Json
来源：http://vus.zhiwuduotai.top

================================================================================
来源：http://vkm.cheryme.top

H. 异常与错误处理
来源：http://vzr.52xcode.cn

================================================================================
来源：http://vpf.dianchejie.cn

[H01] try / catch 基础
来源：http://upy.sysykeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xet.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zyq.redwolf501.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ffy.xuetiantiany.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://skz.yuxming.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gdz.wangdashe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wst.shzxlz.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hhf.zhengqikj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kyi.feifeiyinyue.top

[H02] finally / ensure 收尾
来源：http://cpe.feifeiyinyue.top

Py:   try: f()⏎finally: cleanup()
来源：http://smr.snrcjt.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tmt.guannengcc.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jyt.yueranfly.top

TS:   try { f(); } finally { cleanup(); }
来源：http://krx.jinqigfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://mpl.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://prv.jinqigfzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mns.svipenyu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jif.wangshuangyany.cn

[H03] 主动抛出异常
来源：http://qro.bbcook.cn

Py:   raise ValueError("错误信息")
来源：http://rfk.hcnkem.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yha.sufxvd.cn

JS:   throw new Error("错误信息");
来源：http://ojm.jianghu66.top

TS:   throw new Error("错误信息");
来源：http://ulj.yj20258.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://oag.ivvv.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tsp.vqdsnc.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pee.hysaishi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gtz.jyoumei.cn

[H04] 自定义异常类型
来源：http://rif.zhixingplan.top

Py:   class MyError(Exception): pass
来源：http://awr.jiagoushi.top

PHP:  class MyError extends RuntimeException {}
来源：http://sbo.bjfxy.top

JS:   class MyError extends Error {}
来源：http://xcc.yonumen.top

TS:   class MyError extends Error {}
来源：http://sre.yueranfly.top

Java: class MyException extends RuntimeException {}
来源：http://ujj.dianchejie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nna.dianchejie.cn

Ruby: class MyError < StandardError; end
来源：http://rhn.cashguo.top

C#:   class MyException : Exception {}
来源：http://fbe.ehwqpu.com

[H05] 捕获特定类型
来源：http://vsl.sxryk.cn

Py:   except ValueError as e:
来源：http://zhc.xziqi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hum.cheryme.top

JS:   if (e instanceof TypeError) {}
来源：http://zfp.daxiang520.top

TS:   if (e instanceof TypeError) {}
来源：http://oku.zhijiandao.cn

Java: catch (IOException | SQLException e) {}
来源：http://ugj.zdqjudy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gyi.xingfuxueyuan.xyz

Ruby: rescue ArgumentError => e
来源：http://wkj.yuanzhike.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ppk.sufxvd.cn

[H06] 可选值 / 空值安全访问
来源：http://wik.epnwcf.com

Py:   value = d.get("k") or default
来源：http://fds.fanxiaobao.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://cvn.ywan-chungtsiang.top

JS:   obj?.a?.b;  d ?? default
来源：http://dla.yj202588.top

TS:   obj?.a?.b;  d ?? default
来源：http://fsj.bbcook.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uwi.yfazqb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://zze.guowangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://hck.tianlin.xyz

C#:   obj?.A?.B ?? default
来源：http://uwh.xziqi.cn

[H07] 断言
来源：http://bxy.sysykeji.top

Py:   assert x > 0, "必须为正"
来源：http://wao.snrcjt.cn

PHP:  assert($x > 0);
来源：http://xpd.dianchejie.cn

JS:   console.assert(x > 0);
来源：http://kdx.yangfankeji.com

TS:   console.assert(x > 0);
来源：http://qlu.uphjek.com

Java: assert x > 0 : "必须为正";
来源：http://uxh.kuanghao11.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://alq.snrcjt.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gsy.jinqigufen.top

C#:   Debug.Assert(x > 0);
来源：http://rsa.ywan-chungtsiang.top

[H08] 获取错误信息与堆栈
来源：http://dyb.ppjwa.cn

Py:   str(e);  traceback.format_exc()
来源：http://orf.cucudq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lnl.vqdsnc.cn

JS:   e.message;  e.stack
来源：http://omc.jinqigufen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://sjj.zhixingplan.top

Java: e.getMessage();  e.printStackTrace()
来源：http://qst.ehwqpu.com

Go:   err.Error()
来源：http://ynp.tarul.cn

Ruby: e.message;  e.backtrace
来源：http://pta.iojbl.cn

C#:   e.Message;  e.StackTrace
来源：http://bcw.yuanzhike.top

[H09] 带错误码的异常
来源：http://sxd.guannengcc.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://euk.chenlongwang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lyy.nanxuanxn.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://toz.shanyushiyangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://aml.bbcook.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://svm.iojbl.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lov.xziqi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ohw.nwbrower.top

C#:   // 自定义异常类中加 Code 属性
来源：http://nxt.quarkkingdee.top

[H10] 资源自动释放
来源：http://vil.shanyushiyangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kmn.xinyue.icu

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mym.yueranfly.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xqw.jqgfzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bsk.kuanghao11.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xvw.cheryme.top

Go:   defer f.Close()
来源：http://okn.cdnleiting.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kfv.bbcook.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rvm.aizwys.cn

================================================================================
来源：http://cus.nwbrower.top

I. 正则表达式
来源：http://beo.shzxlz.cn

================================================================================
来源：http://cyd.vqdsnc.cn

[I01] 判断是否匹配
来源：http://bmn.ehwqpu.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hqg.sufxvd.cn

PHP:  preg_match('/\d+/', $s);
来源：http://epq.52xcode.cn

JS:   /\d+/.test(s)
来源：http://ozd.chenjidiqi.icu

TS:   /\d+/.test(s)
来源：http://qrc.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qre.dashuyun.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://izh.zhijiandao.cn

Ruby: s.match?(/\d+/)
来源：http://thd.sxryk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xzu.guannengcc.top

[I02] 提取所有匹配
来源：http://oey.jinqigufen.top

Py:   re.findall(r"\d+", s)
来源：http://akj.xylfe.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hom.feifeiyinyue.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pad.svipenyu.cn

TS:   s.match(/\d+/g)
来源：http://hvk.fengsongda.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mum.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ydw.gzhubu.top

Ruby: s.scan(/\d+/)
来源：http://lxf.sysykeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rxr.yueranfly.top

[I03] 提取捕获分组
来源：http://ytt.vqdsnc.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zvk.xinyue.icu

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mfn.jinqigfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sok.tian-w.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://esb.vqdsnc.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sca.shuidangran.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yvk.nwbrower.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ovh.shuidangran.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kzz.snrcjt.cn

[I04] 正则替换
来源：http://fhi.yfazqb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://oqx.ehwqpu.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eyb.sufxvd.cn

JS:   s.replace(/\d+/g, "#")
来源：http://njt.sufxvd.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yfq.quarkkingdee.top

Java: s.replaceAll("\\d+", "#")
来源：http://elt.jiagoushi.top

Go:   re.ReplaceAllString(s, "#")
来源：http://fhv.jqgufenzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ukf.bjfxy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://whl.0kj1m.cn

[I05] 按正则拆分
来源：http://wma.ehwqpu.com

Py:   re.split(r"\s*,\s*", s)
来源：http://vfo.vqdsnc.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lus.xuanzx.com

JS:   s.split(/\s*,\s*/)
来源：http://xyr.vehdjk.com

TS:   s.split(/\s*,\s*/)
来源：http://kxa.0kj1m.cn

Java: s.split("\\s*,\\s*")
来源：http://eol.sweek.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hyi.daxiang520.top

Ruby: s.split(/\s*,\s*/)
来源：http://xwl.52xcode.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oru.quarkkingdee.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://whz.aibaodan.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yvi.jianghu66.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cma.nanxinkj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wsp.zhixingplan.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rum.zhongyouzk.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cdw.xziqi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cyn.zhaomingkeji.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kke.feifeiyinyue.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://naj.hywenlv.cn

[I07] 忽略大小写与多行模式
来源：http://zci.yueranfly.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wgj.kuanghao11.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kkz.pycfn.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gjo.gaohongyu789.top

TS:   /error/gim
来源：http://yin.jqgfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sof.0kj1m.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kqs.smart0.xyz

Ruby: s.scan(/error/i)
来源：http://oje.jinqigfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xnm.uphjek.com

[I08] 贪婪与非贪婪匹配
来源：http://cew.chenzaomai.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mfw.feifeiyinyue.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kgx.cqqwz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cgm.yuanzhike.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fvn.epnwcf.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://bni.zycfv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xqf.hnqzz.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kkl.shanyushiyangtech.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gpr.jinqigufen.top

================================================================================
来源：http://aeq.zdbjq.cn

J. 日期与时间
来源：http://wvh.iojbl.cn

================================================================================
来源：http://jid.ehwqpu.com

[J01] 获取当前时间
来源：http://kjz.quarkkingdee.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://aqf.xuanzx.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://smq.nanxinkj.top

JS:   new Date();  Date.now()
来源：http://now.vqdsnc.cn

TS:   new Date();  Date.now()
来源：http://vsx.xinyue.icu

Java: LocalDateTime.now();  Instant.now()
来源：http://iyi.guowangkeji.top

Go:   time.Now()
来源：http://xlg.xylfe.cn

Ruby: Time.now
来源：http://qld.yuanzhike.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xkv.0kj1m.cn

[J02] 格式化输出
来源：http://oal.ydjk.org.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dua.andypj.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zll.jyoumei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kiy.ehwqpu.com

TS:   d.toISOString()
来源：http://jyr.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fna.yfazqb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pyf.shzxlz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mkd.wangdashe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hsi.gotoacloud.top

[J03] 字符串解析为日期
来源：http://ixy.xuanzx.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hfk.jianghu66.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bec.chenjidiqi.icu

JS:   new Date("2024-01-02")
来源：http://hmd.0kj1m.cn

TS:   new Date("2024-01-02")
来源：http://tia.cashguo.top

Java: LocalDate.parse("2024-01-02")
来源：http://mjv.ybcxt.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://brp.xuetiantiany.cn

Ruby: Date.parse("2024-01-02")
来源：http://tbf.zhijiandao.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uqk.yongpay.top

[J04] 时间戳与日期互转
来源：http://smg.hysaishi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bzt.meibo888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://onb.gaohongyu789.top


<!-- 参考信息 -->