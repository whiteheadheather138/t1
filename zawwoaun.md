代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://vjc.zycfv.cn

Java: @Override String greet() { return "admin"; }
来源：http://ipt.pengpengdd.cyou

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mqs.aizwys.cn

Ruby: def greet; "admin"; end
来源：http://fwa.gotoacloud.top

C#:   public override string Greet() => "admin";
来源：http://sbi.hesvh.cn

[G07] 调用父类方法
来源：http://cdb.jlsjyb.cn

Py:   super().greet()
来源：http://chq.yj20258.top

PHP:  parent::greet();
来源：http://gvu.cashguo.top

JS:   super.greet();
来源：http://gnu.fehbvm.com

TS:   super.greet();
来源：http://vai.fktsv.cn

Java: super.greet();
来源：http://aop.aizwys.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://czp.ehwqpu.com

Ruby: super
来源：http://vup.xingfuxueyuan.xyz

C#:   base.Greet();
来源：http://lco.pycfn.com

[G08] 静态方法与属性
来源：http://zjy.jqgufenzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kfj.iojbl.cn

PHP:  public static function f() {}
来源：http://bhf.yj202588.top

JS:   static f() {}
来源：http://pbv.jinyuanbaomall.cn

TS:   static f(): void {}
来源：http://pmq.ydzc1.top

Java: static void f() {}
来源：http://byn.cdnleiting.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://vxc.9152youxi.cn

Ruby: def self.f; end
来源：http://idd.bjfxy.top

C#:   public static void F() {}
来源：http://iqg.jinghuilouyu.cn

[G09] 接口 / 抽象类
来源：http://uyu.yuanzhike.top

Py:   from abc import ABC, abstractmethod
来源：http://fsb.yanxiufei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dpi.zycfv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qcu.shangyingyoupin.top

TS:   interface Shape { area(): number; }
来源：http://tpy.jinqigufen.top

Java: interface Shape { double area(); }
来源：http://oxi.yj202588.top

Go:   type Shape interface { Area() float64 }
来源：http://kem.gotoacloud.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://imt.ehwqpu.com

C#:   interface IShape { double Area(); }
来源：http://vaf.ppjwa.cn

[G10] 访问控制
来源：http://ihz.c1oappe.top

Py:   约定 _protected / __private（不强制）
来源：http://kmw.guannengcc.top

PHP:  public / protected / private
来源：http://auy.vehdjk.com

JS:   #private 字段；其余公开
来源：http://hsq.zhengqikj.top

TS:   public / protected / private
来源：http://iil.ydjk.org.cn

Java: public / protected / private / 默认包级
来源：http://ebg.jinghuilouyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ahl.xylfe.cn

Ruby: public / protected / private
来源：http://soj.gzhubu.top

C#:   public / protected / private / internal
来源：http://scn.bjfxy.top

[G11] getter / setter
来源：http://mod.gogol.net.cn

Py:   @property 与 @x.setter
来源：http://nlv.havefunace.top

PHP:  public function getName(): string { return $this->name; }
来源：http://uzo.wangdashe.top

JS:   get name() { return this._name; }
来源：http://lur.guannengcc.top

TS:   get name(): string { return this._name; }
来源：http://qod.aizwys.cn

Java: public String getName() { return name; }
来源：http://fty.gotoacloud.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hlg.jyoumei.cn

Ruby: attr_accessor :name
来源：http://rll.epnwcf.com

C#:   public string Name { get; set; }
来源：http://tgp.yuxming.cn

[G12] 对象转字符串
来源：http://brp.jlsjyb.cn

Py:   def __str__(self): return self.name
来源：http://zct.tian-w.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tzf.sysykeji.top

JS:   toString() { return this.name; }
来源：http://iar.gotoacloud.top

TS:   toString(): string { return this.name; }
来源：http://gby.0kj1m.cn

Java: @Override public String toString() { return name; }
来源：http://hhs.tarul.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kpm.gotoacloud.top

Ruby: def to_s; @name; end
来源：http://tnd.zycfv.cn

C#:   public override string ToString() => Name;
来源：http://ysc.zdqjudy.top

[G13] 判断对象类型
来源：http://ill.iojbl.cn

Py:   isinstance(u, User)
来源：http://kxf.ivvv.top

PHP:  $u instanceof User
来源：http://kgm.cucudq.cn

JS:   u instanceof User
来源：http://oaq.yangfankeji.com

TS:   u instanceof User
来源：http://idh.zhiwuduotai.top

Java: u instanceof User
来源：http://iqd.quarkkingdee.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lrj.xuanzx.com

Ruby: u.is_a?(User)
来源：http://hyg.yvedp.cn

C#:   u is User
来源：http://vsx.hammf.cn

[G14] 数据类 / record
来源：http://dil.ydjk.org.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fxy.zhijiandao.cn

PHP:  // 用 readonly 属性模拟
来源：http://zsv.xuanzx.com

JS:   // 无内置：普通类或对象字面量
来源：http://zad.bbcook.cn

TS:   type User = { name: string; age: number };
来源：http://biq.tarul.cn

Java: record User(String name, int age) {}
来源：http://zju.dashuyun.cn

Go:   type User struct { Name string; Age int }
来源：http://zhc.zhengqikj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yjr.yanxiufei.cn

C#:   record User(string Name, int Age);
来源：http://opq.cdnleiting.top

[G15] 枚举
来源：http://zta.nanxuanxn.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wit.dashuyun.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xhk.chenzaomai.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cfs.xingfuxueyuan.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://itp.jinyuanbaomall.cn

Java: enum Color { RED, GREEN }
来源：http://oqs.shzxlz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gyl.pengpengdd.cyou

Ruby: Color = %i[red green].freeze
来源：http://osr.pycfn.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://emb.cheryme.top

[G16] 对象转数组 / 字典
来源：http://tap.zhixingplan.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ynk.quarkkingdee.top

PHP:  get_object_vars($obj);
来源：http://rrm.ydjk.org.cn

JS:   Object.entries(obj)
来源：http://kij.yvedp.cn

TS:   Object.entries(obj)
来源：http://fdb.xinyue.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oqe.ppjwa.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yyy.zhaomingkeji.xyz

Ruby: obj.instance_variables
来源：http://qpj.aibaodan.cn

C#:   // 用反射或 System.Text.Json
来源：http://uuk.cdnleiting.top

================================================================================
来源：http://ovm.yanxiufei.cn

H. 异常与错误处理
来源：http://yhx.zdbjq.cn

================================================================================
来源：http://lyy.pycfn.com

[H01] try / catch 基础
来源：http://bfg.yj20258888.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://buc.tian-w.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ywi.bjfxy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ohf.shangyingyoupin.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dhq.dashuyun.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qpg.yj20258888.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://byk.sjlbkw.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rah.aibaodan.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uiw.316326.xyz

[H02] finally / ensure 收尾
来源：http://rui.52xcode.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kym.xuanzx.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://abr.epnwcf.com

JS:   try { f(); } finally { cleanup(); }
来源：http://tcd.hcnkem.com

TS:   try { f(); } finally { cleanup(); }
来源：http://dov.nwbrower.top

Java: try { f(); } finally { cleanup(); }
来源：http://ccn.shangyingyoupin.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://djv.ivvv.top

Ruby: begin; f; ensure; cleanup; end
来源：http://abf.zdbjq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qfv.dianchejie.cn

[H03] 主动抛出异常
来源：http://kkm.jinqigufen.top

Py:   raise ValueError("错误信息")
来源：http://qkv.aizwys.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fyr.fengsongda.top

JS:   throw new Error("错误信息");
来源：http://iam.jqgfzy.top

TS:   throw new Error("错误信息");
来源：http://fxn.feifeiyinyue.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://evp.zdqjudy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wdq.dianchejie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gnn.chenzaomai.com

C#:   throw new ArgumentException("错误信息");
来源：http://mal.zhengqikj.top

[H04] 自定义异常类型
来源：http://hkr.tanke756.top

Py:   class MyError(Exception): pass
来源：http://ypy.yonumen.top

PHP:  class MyError extends RuntimeException {}
来源：http://zxt.ybcxt.top

JS:   class MyError extends Error {}
来源：http://ffd.zdqjudy.top

TS:   class MyError extends Error {}
来源：http://aup.jinghuilouyu.cn

Java: class MyException extends RuntimeException {}
来源：http://rdl.chenlongwang.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zfl.tarul.cn

Ruby: class MyError < StandardError; end
来源：http://ugv.zhijiandao.cn

C#:   class MyException : Exception {}
来源：http://ftv.sxryk.cn

[H05] 捕获特定类型
来源：http://rfe.tian-w.cn

Py:   except ValueError as e:
来源：http://vsa.fengsongda.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://upe.tian-w.cn

JS:   if (e instanceof TypeError) {}
来源：http://crz.zhoulong.xyz

TS:   if (e instanceof TypeError) {}
来源：http://rtj.jinqigfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://qyn.tanke756.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jdz.jinqigfzy.top

Ruby: rescue ArgumentError => e
来源：http://ogb.jqgfzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lky.ydjk.org.cn

[H06] 可选值 / 空值安全访问
来源：http://zsw.cheryme.top

Py:   value = d.get("k") or default
来源：http://bgy.ybcxt.top

PHP:  $v = $d["k"] ?? null;
来源：http://izw.yuxming.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fkp.redwolf501.top

TS:   obj?.a?.b;  d ?? default
来源：http://wwt.gaohongyu789.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zxv.yj20258.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wua.shanyushiyangtech.top

Ruby: d&.dig(:a, :b)
来源：http://fqi.zycfv.cn

C#:   obj?.A?.B ?? default
来源：http://amy.meibo888.top

[H07] 断言
来源：http://zpa.zhijiandao.cn

Py:   assert x > 0, "必须为正"
来源：http://ohj.ydzc1.top

PHP:  assert($x > 0);
来源：http://ymt.ywan-chungtsiang.top

JS:   console.assert(x > 0);
来源：http://ued.cheryme.top

TS:   console.assert(x > 0);
来源：http://ewd.andypj.xyz

Java: assert x > 0 : "必须为正";
来源：http://krb.cheryme.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gpk.ywan-chungtsiang.top

Ruby: raise "必须为正" unless x > 0
来源：http://skf.feifeiyinyue.top

C#:   Debug.Assert(x > 0);
来源：http://kcn.ydjk.org.cn

[H08] 获取错误信息与堆栈
来源：http://biu.yj202588.top

Py:   str(e);  traceback.format_exc()
来源：http://uxu.ctjpmb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hvg.jyoumei.cn

JS:   e.message;  e.stack
来源：http://qrf.jiagoushi.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lte.pengpengdd.cyou

Java: e.getMessage();  e.printStackTrace()
来源：http://mdc.yangfankeji.com

Go:   err.Error()
来源：http://owm.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://alh.havefunace.top

C#:   e.Message;  e.StackTrace
来源：http://wuo.nwbrower.top

[H09] 带错误码的异常
来源：http://vyp.vqdsnc.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://alw.hfpthk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bml.fengsongda.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xgr.cheryme.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://swk.sxryk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ayy.chenzaomai.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yha.chenjidiqi.icu

Ruby: raise MyError.new("fail", 500)
来源：http://fzm.jianghu66.top

C#:   // 自定义异常类中加 Code 属性
来源：http://roy.wangdashe.top

[H10] 资源自动释放
来源：http://nsq.jqgfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://nnp.zdqjudy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qkl.sufxvd.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lsf.guowangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ars.yanxiufei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wao.ivvv.top

Go:   defer f.Close()
来源：http://mnk.aizwys.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cdf.jinqigfzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kiw.pengpengdd.cyou

================================================================================
来源：http://fgq.yfazqb.com

I. 正则表达式
来源：http://aui.bjfxy.top

================================================================================
来源：http://ttr.uphjek.com

[I01] 判断是否匹配
来源：http://xxc.haohaochexian.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bjv.yonumen.top

PHP:  preg_match('/\d+/', $s);
来源：http://ssm.chenlongwang.top

JS:   /\d+/.test(s)
来源：http://jyr.xingfuxueyuan.xyz

TS:   /\d+/.test(s)
来源：http://mop.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zgc.dashuyun.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lqv.cheryme.top

Ruby: s.match?(/\d+/)
来源：http://ycm.ywan-chungtsiang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ssl.epnwcf.com

[I02] 提取所有匹配
来源：http://ywp.xylfe.cn

Py:   re.findall(r"\d+", s)
来源：http://ugg.ybcxt.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://huv.sweek.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jmo.chenzaomai.com

TS:   s.match(/\d+/g)
来源：http://upv.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pbz.ydjk.org.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qat.ivvv.top

Ruby: s.scan(/\d+/)
来源：http://ien.hfpthk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gjp.xziqi.cn

[I03] 提取捕获分组
来源：http://pnq.nwbrower.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gyg.hnqzz.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bqt.fengsongda.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vbb.xingfuxueyuan.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ixw.gotoacloud.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qtg.snrcjt.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hjs.hongshengwenyu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vep.cheryme.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mtz.fktsv.cn

[I04] 正则替换
来源：http://hdt.c1oappe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://dgg.jiagoushi.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://igr.shanyushiyangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://usw.daxiang520.top

TS:   s.replace(/\d+/g, "#")
来源：http://day.meibo888.top

Java: s.replaceAll("\\d+", "#")
来源：http://pbo.svipenyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oxa.cheryme.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hpf.9152youxi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://stp.vehdjk.com

[I05] 按正则拆分
来源：http://gfu.yangfankeji.com

Py:   re.split(r"\s*,\s*", s)
来源：http://xow.wangdashe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wxt.shuidangran.top

JS:   s.split(/\s*,\s*/)
来源：http://pco.uphjek.com

TS:   s.split(/\s*,\s*/)
来源：http://kum.ydjk.org.cn

Java: s.split("\\s*,\\s*")
来源：http://zdc.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nqf.shuidangran.top

Ruby: s.split(/\s*,\s*/)
来源：http://ysk.jianghu66.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rqp.zhongyouzk.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dkz.sysykeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ixr.jqgfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vbj.jinyuanbaomall.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jco.haohaochexian.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uac.jiagoushi.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nkw.nwbrower.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://acd.ydzc1.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bml.cucudq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tev.cheryme.top

[I07] 忽略大小写与多行模式
来源：http://ndw.pycfn.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pgm.xuetiantiany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hdx.guowangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pxr.yvedp.cn

TS:   /error/gim
来源：http://isg.feifeiyinyue.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xep.wangdashe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bhr.jyoumei.cn

Ruby: s.scan(/error/i)
来源：http://cnh.fktsv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zft.jlsjyb.cn

[I08] 贪婪与非贪婪匹配
来源：http://qwz.uphjek.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ifr.fzhhl.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xwz.pycfn.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wdg.wangshuangyany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jih.yuxming.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vgl.vqdsnc.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://voq.sufxvd.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ghs.hesvh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cia.kuanghao11.cn

================================================================================
来源：http://wiy.jyoumei.cn

J. 日期与时间
来源：http://aus.aibaodan.cn

================================================================================
来源：http://eac.hnxiangtu.top

[J01] 获取当前时间
来源：http://ibd.hongshengwenyu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://yuj.hywenlv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cea.yj20258.top

JS:   new Date();  Date.now()
来源：http://scu.quarkkingdee.top

TS:   new Date();  Date.now()
来源：http://rgc.zdqjudy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qqa.zhixingplan.top

Go:   time.Now()
来源：http://fhz.chenjidiqi.icu

Ruby: Time.now
来源：http://foy.yongpay.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bvt.cdnleiting.top

[J02] 格式化输出
来源：http://bqp.dashuyun.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wbr.cucudq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vxt.sweek.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dej.uphjek.com

TS:   d.toISOString()
来源：http://ubc.316326.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mcv.ivvv.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://npz.0kj1m.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qro.sweek.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dlc.aibaodan.cn

[J03] 字符串解析为日期
来源：http://okx.iojbl.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://apm.shuidangran.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vcg.ppjwa.cn

JS:   new Date("2024-01-02")
来源：http://uzh.shzxlz.cn

TS:   new Date("2024-01-02")
来源：http://tos.jinqigfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://uid.yangfankeji.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qup.gogol.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://qnz.sjlbkw.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://txq.ydzc1.top

[J04] 时间戳与日期互转
来源：http://myf.zdbjq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fbu.xinyue.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ahg.ivvv.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gnq.hammf.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kmd.zycfv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pzq.hesvh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qqh.birdmap.top


<!-- 参考信息 -->