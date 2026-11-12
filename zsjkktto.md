代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://bxn.quarkkingdee.top

[G07] 调用父类方法
来源：http://ylk.yvedp.cn

Py:   super().greet()
来源：http://lvn.havefunace.top

PHP:  parent::greet();
来源：http://qnc.cqqwz.cn

JS:   super.greet();
来源：http://sbj.jlsjyb.cn

TS:   super.greet();
来源：http://uhc.feifeiyinyue.top

Java: super.greet();
来源：http://rlf.redwolf501.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bht.andypj.xyz

Ruby: super
来源：http://fqn.hammf.cn

C#:   base.Greet();
来源：http://hbj.zhaomingkeji.xyz

[G08] 静态方法与属性
来源：http://zcv.zycfv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://umb.316326.xyz

PHP:  public static function f() {}
来源：http://rch.shanyushiyangkeji.top

JS:   static f() {}
来源：http://xds.iojbl.cn

TS:   static f(): void {}
来源：http://qqh.hammf.cn

Java: static void f() {}
来源：http://jgv.nanxuanxn.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://iyg.yvedp.cn

Ruby: def self.f; end
来源：http://swo.c1oappe.top

C#:   public static void F() {}
来源：http://wwe.pycfn.com

[G09] 接口 / 抽象类
来源：http://tbd.xingfuxueyuan.xyz

Py:   from abc import ABC, abstractmethod
来源：http://fnm.yuanzhike.top

PHP:  interface Shape { public function area(): float; }
来源：http://lrj.yfazqb.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://igb.feifeiyinyue.top

TS:   interface Shape { area(): number; }
来源：http://fxc.cdnleiting.top

Java: interface Shape { double area(); }
来源：http://scb.jinghuilouyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://gxg.ivvv.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dcg.yangfankeji.com

C#:   interface IShape { double Area(); }
来源：http://jvr.xingfuxueyuan.xyz

[G10] 访问控制
来源：http://tcr.cqqwz.cn

Py:   约定 _protected / __private（不强制）
来源：http://yfh.c1oappe.top

PHP:  public / protected / private
来源：http://cue.shzxlz.cn

JS:   #private 字段；其余公开
来源：http://cdc.shangyingyoupin.top

TS:   public / protected / private
来源：http://mpn.xinyue.icu

Java: public / protected / private / 默认包级
来源：http://rgg.xuetiantiany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pqz.ppjwa.cn

Ruby: public / protected / private
来源：http://pny.xziqi.cn

C#:   public / protected / private / internal
来源：http://gpg.ybcxt.top

[G11] getter / setter
来源：http://pyv.jinqigfzy.top

Py:   @property 与 @x.setter
来源：http://klg.ydzc1.top

PHP:  public function getName(): string { return $this->name; }
来源：http://gae.sjlbkw.cn

JS:   get name() { return this._name; }
来源：http://lga.gaohongyu789.top

TS:   get name(): string { return this._name; }
来源：http://gzw.gaohongyu789.top

Java: public String getName() { return name; }
来源：http://bsg.yongpay.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://atu.snrcjt.cn

Ruby: attr_accessor :name
来源：http://hvv.jinqigufen.top

C#:   public string Name { get; set; }
来源：http://urv.hammf.cn

[G12] 对象转字符串
来源：http://yvr.hysaishi.cn

Py:   def __str__(self): return self.name
来源：http://vmo.hnxiangtu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rux.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://tte.52xcode.cn

TS:   toString(): string { return this.name; }
来源：http://thz.fzhhl.top

Java: @Override public String toString() { return name; }
来源：http://rbb.smart0.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://ths.shzxlz.cn

Ruby: def to_s; @name; end
来源：http://yuf.zdqjudy.top

C#:   public override string ToString() => Name;
来源：http://hdx.jiagoushi.top

[G13] 判断对象类型
来源：http://eao.nwbrower.top

Py:   isinstance(u, User)
来源：http://bcs.uphjek.com

PHP:  $u instanceof User
来源：http://nrr.ydzc1.top

JS:   u instanceof User
来源：http://rcz.sxryk.cn

TS:   u instanceof User
来源：http://kzz.tianlin.xyz

Java: u instanceof User
来源：http://qew.yj20258.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vka.yj20258888.top

Ruby: u.is_a?(User)
来源：http://ufy.sxryk.cn

C#:   u is User
来源：http://onf.fktsv.cn

[G14] 数据类 / record
来源：http://oyw.jinghuilouyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://orw.dianchejie.cn

PHP:  // 用 readonly 属性模拟
来源：http://dka.hongshengwenyu.top

JS:   // 无内置：普通类或对象字面量
来源：http://fpg.zhiwuduotai.top

TS:   type User = { name: string; age: number };
来源：http://ibi.sweek.top

Java: record User(String name, int age) {}
来源：http://iia.jianghu66.top

Go:   type User struct { Name string; Age int }
来源：http://tcp.yj20258.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dpj.yuanzhike.top

C#:   record User(string Name, int Age);
来源：http://vjz.jiagoushi.top

[G15] 枚举
来源：http://ykd.yuanzhike.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vaq.gzhubu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ilz.jianghu66.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://loq.xingfuxueyuan.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qqe.cheryme.top

Java: enum Color { RED, GREEN }
来源：http://epe.52xcode.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cnc.tarul.cn

Ruby: Color = %i[red green].freeze
来源：http://gkv.yongpay.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qzn.hcnkem.com

[G16] 对象转数组 / 字典
来源：http://fpd.chenzaomai.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xam.jianghu66.top

PHP:  get_object_vars($obj);
来源：http://bmu.nanxuanxn.top

JS:   Object.entries(obj)
来源：http://src.sxryk.cn

TS:   Object.entries(obj)
来源：http://dmg.shuidangran.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wfj.zhijiandao.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://smh.zycfv.cn

Ruby: obj.instance_variables
来源：http://tdw.ydjk.org.cn

C#:   // 用反射或 System.Text.Json
来源：http://ogv.zhaomingkeji.xyz

================================================================================
来源：http://tzf.birdmap.top

H. 异常与错误处理
来源：http://taa.ydzc1.top

================================================================================
来源：http://frq.guowangkeji.top

[H01] try / catch 基础
来源：http://ciq.hcnkem.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ewe.xingfuxueyuan.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xrf.hysaishi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jht.hysaishi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://foz.sysykeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oik.yvedp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yro.bbcook.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gnh.jinghuilouyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bhl.hfpthk.cn

[H02] finally / ensure 收尾
来源：http://mzl.cheryme.top

Py:   try: f()⏎finally: cleanup()
来源：http://sed.hywenlv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://oxc.zhaomingkeji.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://rko.sxryk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://joq.xinyue.icu

Java: try { f(); } finally { cleanup(); }
来源：http://lin.xuetiantiany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vok.xuetiantiany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wya.jqgfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ggu.cashguo.top

[H03] 主动抛出异常
来源：http://csg.xuanzx.com

Py:   raise ValueError("错误信息")
来源：http://siz.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://czp.cqqwz.cn

JS:   throw new Error("错误信息");
来源：http://hen.zdqjudy.top

TS:   throw new Error("错误信息");
来源：http://brj.guowangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dqy.chenlongwang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mbu.feifeiyinyue.top

Ruby: raise ArgumentError, "错误信息"
来源：http://wjx.gogol.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hjq.ppjwa.cn

[H04] 自定义异常类型
来源：http://pft.jlsjyb.cn

Py:   class MyError(Exception): pass
来源：http://elx.zdqjudy.top

PHP:  class MyError extends RuntimeException {}
来源：http://nga.cashguo.top

JS:   class MyError extends Error {}
来源：http://jid.xingfuxueyuan.xyz

TS:   class MyError extends Error {}
来源：http://yjc.chenzaomai.com

Java: class MyException extends RuntimeException {}
来源：http://oqa.yangfankeji.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sjh.zdbjq.cn

Ruby: class MyError < StandardError; end
来源：http://qeq.jqgfzy.top

C#:   class MyException : Exception {}
来源：http://lhi.hcnkem.com

[H05] 捕获特定类型
来源：http://hlm.fktsv.cn

Py:   except ValueError as e:
来源：http://qje.sxryk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cdo.hnqzz.top

JS:   if (e instanceof TypeError) {}
来源：http://huy.yongpay.top

TS:   if (e instanceof TypeError) {}
来源：http://clg.sysykeji.top

Java: catch (IOException | SQLException e) {}
来源：http://ozs.0kj1m.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bkj.c1oappe.top

Ruby: rescue ArgumentError => e
来源：http://eup.yonumen.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kvv.yvedp.cn

[H06] 可选值 / 空值安全访问
来源：http://pgs.yfazqb.com

Py:   value = d.get("k") or default
来源：http://niw.xuetiantiany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jxd.cqqwz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lzb.tianlin.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://hxx.jinqigfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ilw.shuidangran.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fyo.sufxvd.cn

Ruby: d&.dig(:a, :b)
来源：http://mgr.cashguo.top

C#:   obj?.A?.B ?? default
来源：http://qfm.xinyue.icu

[H07] 断言
来源：http://qlh.hesvh.cn

Py:   assert x > 0, "必须为正"
来源：http://gnc.tanke756.top

PHP:  assert($x > 0);
来源：http://hwe.chenlongwang.top

JS:   console.assert(x > 0);
来源：http://byz.tian-w.cn

TS:   console.assert(x > 0);
来源：http://fhv.zhongyouzk.top

Java: assert x > 0 : "必须为正";
来源：http://gva.sjlbkw.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dwa.meibo888.top

Ruby: raise "必须为正" unless x > 0
来源：http://yyy.hnxiangtu.top

C#:   Debug.Assert(x > 0);
来源：http://snj.hcnkem.com

[H08] 获取错误信息与堆栈
来源：http://akp.hongshengwenyu.top

Py:   str(e);  traceback.format_exc()
来源：http://dxd.wangdashe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ibj.tianlin.xyz

JS:   e.message;  e.stack
来源：http://hpr.ydjk.org.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dtv.pengpengdd.cyou

Java: e.getMessage();  e.printStackTrace()
来源：http://efj.sweek.top

Go:   err.Error()
来源：http://rrh.yvedp.cn

Ruby: e.message;  e.backtrace
来源：http://shs.tanke756.top

C#:   e.Message;  e.StackTrace
来源：http://cmx.jqgufenzy.top

[H09] 带错误码的异常
来源：http://afp.nwbrower.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qsz.chenzaomai.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://bch.zhiwuduotai.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uhe.52xcode.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vnd.xylfe.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://djf.havefunace.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nns.cucudq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kcj.ehwqpu.com

C#:   // 自定义异常类中加 Code 属性
来源：http://hxp.gzhubu.top

[H10] 资源自动释放
来源：http://rug.meibo888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://crk.zycfv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bhq.hysaishi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ysx.ybcxt.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wyp.fktsv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xwx.zhaomingkeji.xyz

Go:   defer f.Close()
来源：http://xzt.jqgfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ssl.guowangkeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tff.fanxiaobao.xyz

================================================================================
来源：http://orz.meibo888.top

I. 正则表达式
来源：http://srf.daria6918.cn

================================================================================
来源：http://ocn.havefunace.top

[I01] 判断是否匹配
来源：http://pec.sxryk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pas.jyoumei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hxo.zycfv.cn

JS:   /\d+/.test(s)
来源：http://oks.0kj1m.cn

TS:   /\d+/.test(s)
来源：http://bvv.fzhhl.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://irg.vehdjk.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ecg.ydzc1.top

Ruby: s.match?(/\d+/)
来源：http://uiu.yuxming.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ksb.jyoumei.cn

[I02] 提取所有匹配
来源：http://pfn.fanxiaobao.xyz

Py:   re.findall(r"\d+", s)
来源：http://qid.fengsongda.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://src.guannengcc.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://glv.cqqwz.cn

TS:   s.match(/\d+/g)
来源：http://eey.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cgb.wangdashe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jmb.svipenyu.cn

Ruby: s.scan(/\d+/)
来源：http://yod.xuanzx.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kue.jinqigfzy.top

[I03] 提取捕获分组
来源：http://znt.pengpengdd.cyou

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nrt.ydzc1.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qcu.ywan-chungtsiang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://geq.gaohongyu789.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wrd.quarkkingdee.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bnz.chenlongwang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cuq.yuanzhike.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mrm.pycfn.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xmg.hywenlv.cn

[I04] 正则替换
来源：http://qnu.hcnkem.com

Py:   re.sub(r"\d+", "#", s)
来源：http://uwm.ydjk.org.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kjc.ybcxt.top

JS:   s.replace(/\d+/g, "#")
来源：http://ijp.yonumen.top

TS:   s.replace(/\d+/g, "#")
来源：http://mlh.aibaodan.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hdm.yonumen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://owe.bjfxy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qtr.tarul.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dlc.daxiang520.top

[I05] 按正则拆分
来源：http://iwc.sxryk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ydm.shuidangran.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bkg.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://iih.shanyushiyangtech.top

TS:   s.split(/\s*,\s*/)
来源：http://baz.snrcjt.cn

Java: s.split("\\s*,\\s*")
来源：http://hkr.haohaochexian.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bhz.0kj1m.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yrm.jinqigufen.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ekh.xuanzx.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dfv.iojbl.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xps.hnqzz.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fzf.aibaodan.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rzs.ctjpmb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kvj.fanxiaobao.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vsg.tanke756.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pnn.hammf.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jua.daxiang520.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rnb.xuetiantiany.cn

[I07] 忽略大小写与多行模式
来源：http://uzt.iojbl.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://aov.gogol.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://aru.aibaodan.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xxe.shangyingyoupin.top

TS:   /error/gim
来源：http://kyi.xingfuxueyuan.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ixu.yuanzhike.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://whn.shanyushiyangkeji.top

Ruby: s.scan(/error/i)
来源：http://xbu.bbcook.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qgy.ppjwa.cn

[I08] 贪婪与非贪婪匹配
来源：http://lqw.zycfv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://drj.birdmap.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://stp.xziqi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hjk.smart0.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nqm.jinqigufen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://uyb.zhijiandao.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://emp.gogol.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wsl.yangfankeji.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mhk.9152youxi.cn

================================================================================
来源：http://xng.shuidangran.top

J. 日期与时间
来源：http://dsk.hywenlv.cn

================================================================================
来源：http://ckr.yfazqb.com

[J01] 获取当前时间
来源：http://ret.tanke756.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bfx.bbcook.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://snn.shanyushiyangtech.top

JS:   new Date();  Date.now()
来源：http://jki.tanke756.top

TS:   new Date();  Date.now()
来源：http://qcf.kuanghao11.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gcy.wangshuangyany.cn

Go:   time.Now()
来源：http://ljn.9152youxi.cn

Ruby: Time.now
来源：http://sea.dashuyun.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hml.jqgfzy.top

[J02] 格式化输出
来源：http://lhs.pengpengdd.cyou

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zlw.birdmap.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oup.redwolf501.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tta.quarkkingdee.top

TS:   d.toISOString()
来源：http://epj.nwbrower.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jkl.jinqigufen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rhh.shangyingyoupin.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bnv.zycfv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wnu.andypj.xyz

[J03] 字符串解析为日期
来源：http://iam.guannengcc.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lmq.316326.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://psa.chenzaomai.com

JS:   new Date("2024-01-02")
来源：http://lmg.shanyushiyangkeji.top

TS:   new Date("2024-01-02")
来源：http://iif.redwolf501.top

Java: LocalDate.parse("2024-01-02")
来源：http://ruk.jinyuanbaomall.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pnx.iojbl.cn

Ruby: Date.parse("2024-01-02")
来源：http://yvx.gogol.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fax.zhiwuduotai.top

[J04] 时间戳与日期互转
来源：http://dgt.xziqi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hjm.yuanzhike.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ylk.aizwys.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rbo.shuidangran.top

TS:   Math.floor(Date.now() / 1000)
来源：http://gda.zhixingplan.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mgc.zdbjq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fek.kuanghao11.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ndc.yonumen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zjl.gogol.net.cn

[J05] 时间加减（加 7 天）
来源：http://jcw.316326.xyz

Py:   now + timedelta(days=7)
来源：http://csy.hnxiangtu.top


<!-- 参考信息 -->