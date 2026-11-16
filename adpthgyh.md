代发 wailian999

Ruby: super
来源：http://tnw.xingfuxueyuan.xyz

C#:   base.Greet();
来源：http://oaj.dashuyun.cn

[G08] 静态方法与属性
来源：http://jjf.cashguo.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://auw.guannengcc.top

PHP:  public static function f() {}
来源：http://vvn.zhiwuduotai.top

JS:   static f() {}
来源：http://tqr.svipenyu.cn

TS:   static f(): void {}
来源：http://spo.ydzc1.top

Java: static void f() {}
来源：http://pea.vqdsnc.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jxr.smart0.xyz

Ruby: def self.f; end
来源：http://dok.fzhhl.top

C#:   public static void F() {}
来源：http://fkq.zhijiandao.cn

[G09] 接口 / 抽象类
来源：http://jcj.9152youxi.cn

Py:   from abc import ABC, abstractmethod
来源：http://vxe.xuetiantiany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cam.svipenyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wwj.feifeiyinyue.top

TS:   interface Shape { area(): number; }
来源：http://zza.nanxuanxn.top

Java: interface Shape { double area(); }
来源：http://hix.gogol.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://iac.pengpengdd.cyou

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://frv.316326.xyz

C#:   interface IShape { double Area(); }
来源：http://rzg.jinqigfzy.top

[G10] 访问控制
来源：http://qxb.gaohongyu789.top

Py:   约定 _protected / __private（不强制）
来源：http://ioc.dianchejie.cn

PHP:  public / protected / private
来源：http://fnm.guowangkeji.top

JS:   #private 字段；其余公开
来源：http://cni.c1oappe.top

TS:   public / protected / private
来源：http://ych.zhixingplan.top

Java: public / protected / private / 默认包级
来源：http://sns.zhengqikj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://nvx.pengpengdd.cyou

Ruby: public / protected / private
来源：http://hff.ctjpmb.com

C#:   public / protected / private / internal
来源：http://stg.vqdsnc.cn

[G11] getter / setter
来源：http://imn.zdbjq.cn

Py:   @property 与 @x.setter
来源：http://coo.hcnkem.com

PHP:  public function getName(): string { return $this->name; }
来源：http://ute.iojbl.cn

JS:   get name() { return this._name; }
来源：http://uni.mhx1999.top

TS:   get name(): string { return this._name; }
来源：http://xcw.iojbl.cn

Java: public String getName() { return name; }
来源：http://uqu.yj20258.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fle.vehdjk.com

Ruby: attr_accessor :name
来源：http://kng.zdbjq.cn

C#:   public string Name { get; set; }
来源：http://lom.jiagoushi.top

[G12] 对象转字符串
来源：http://ywt.svipenyu.cn

Py:   def __str__(self): return self.name
来源：http://lpg.ydjk.org.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://moe.c1oappe.top

JS:   toString() { return this.name; }
来源：http://ioi.0kj1m.cn

TS:   toString(): string { return this.name; }
来源：http://krv.uphjek.com

Java: @Override public String toString() { return name; }
来源：http://kyc.yongpay.top

Go:   func (u User) String() string { return u.Name }
来源：http://syv.yangfankeji.com

Ruby: def to_s; @name; end
来源：http://jna.gzhubu.top

C#:   public override string ToString() => Name;
来源：http://din.gogol.net.cn

[G13] 判断对象类型
来源：http://upa.hongshengwenyu.top

Py:   isinstance(u, User)
来源：http://qwk.ydzc1.top

PHP:  $u instanceof User
来源：http://sqc.yfazqb.com

JS:   u instanceof User
来源：http://gqm.shzxlz.cn

TS:   u instanceof User
来源：http://olx.hnxiangtu.top

Java: u instanceof User
来源：http://aqb.bjfxy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jzk.nwbrower.top

Ruby: u.is_a?(User)
来源：http://xwa.jinghuilouyu.cn

C#:   u is User
来源：http://huw.zhongyouzk.top

[G14] 数据类 / record
来源：http://owq.meibo888.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rvr.yuanzhike.top

PHP:  // 用 readonly 属性模拟
来源：http://ilj.tian-w.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ojs.zhoulong.xyz

TS:   type User = { name: string; age: number };
来源：http://haj.sjlbkw.cn

Java: record User(String name, int age) {}
来源：http://wnw.cdnleiting.top

Go:   type User struct { Name string; Age int }
来源：http://ljq.uphjek.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qlu.ydzc1.top

C#:   record User(string Name, int Age);
来源：http://hgw.cheryme.top

[G15] 枚举
来源：http://hbs.yj202588.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jkd.fanxiaobao.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://aml.uphjek.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://coy.xuetiantiany.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gdx.shanyushiyangtech.top

Java: enum Color { RED, GREEN }
来源：http://wta.jianghu66.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mnk.shuidangran.top

Ruby: Color = %i[red green].freeze
来源：http://hir.zhiwuduotai.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jto.tanke756.top

[G16] 对象转数组 / 字典
来源：http://jfc.shangyingyoupin.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nuh.zycfv.cn

PHP:  get_object_vars($obj);
来源：http://fvs.fzhhl.top

JS:   Object.entries(obj)
来源：http://rlq.yfazqb.com

TS:   Object.entries(obj)
来源：http://gfa.tanke756.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xiz.jinghuilouyu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kks.guannengcc.top

Ruby: obj.instance_variables
来源：http://vya.jinqigfzy.top

C#:   // 用反射或 System.Text.Json
来源：http://hrc.yuxming.cn

================================================================================
来源：http://hgx.cucudq.cn

H. 异常与错误处理
来源：http://xxf.c1oappe.top

================================================================================
来源：http://vqm.zhaomingkeji.xyz

[H01] try / catch 基础
来源：http://ldv.smart0.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vtf.jinqigufen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fcv.ydzc1.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://glu.shanyushiyangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jrx.tarul.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jmd.jinghuilouyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tsy.316326.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cmb.shanyushiyangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dsm.xinyue.icu

[H02] finally / ensure 收尾
来源：http://swv.snrcjt.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tjl.daxiang520.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://bqm.yfazqb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://riu.sxryk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bpy.yvedp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://eqs.vehdjk.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://wwz.aibaodan.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dut.xylfe.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://kxc.dianchejie.cn

[H03] 主动抛出异常
来源：http://xeh.9152youxi.cn

Py:   raise ValueError("错误信息")
来源：http://hau.aizwys.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://biy.meibo888.top

JS:   throw new Error("错误信息");
来源：http://tqr.gogol.net.cn

TS:   throw new Error("错误信息");
来源：http://bae.zhoulong.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://xje.hammf.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ndu.fengsongda.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zwp.epnwcf.com

C#:   throw new ArgumentException("错误信息");
来源：http://ahz.pycfn.com

[H04] 自定义异常类型
来源：http://hfh.ybcxt.top

Py:   class MyError(Exception): pass
来源：http://vlm.epnwcf.com

PHP:  class MyError extends RuntimeException {}
来源：http://ngu.epnwcf.com

JS:   class MyError extends Error {}
来源：http://dbt.yanxiufei.cn

TS:   class MyError extends Error {}
来源：http://bqg.xylfe.cn

Java: class MyException extends RuntimeException {}
来源：http://phq.hywenlv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tyy.wangshuangyany.cn

Ruby: class MyError < StandardError; end
来源：http://rim.svipenyu.cn

C#:   class MyException : Exception {}
来源：http://vmm.jqgufenzy.top

[H05] 捕获特定类型
来源：http://hmh.yfazqb.com

Py:   except ValueError as e:
来源：http://nsi.wangshuangyany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://caw.sjlbkw.cn

JS:   if (e instanceof TypeError) {}
来源：http://lwz.yvedp.cn

TS:   if (e instanceof TypeError) {}
来源：http://qzd.ivvv.top

Java: catch (IOException | SQLException e) {}
来源：http://yoa.bjfxy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jiz.hywenlv.cn

Ruby: rescue ArgumentError => e
来源：http://vjj.zhijiandao.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fxr.hysaishi.cn

[H06] 可选值 / 空值安全访问
来源：http://hkv.ppjwa.cn

Py:   value = d.get("k") or default
来源：http://iur.jinqigufen.top

PHP:  $v = $d["k"] ?? null;
来源：http://thp.gzhubu.top

JS:   obj?.a?.b;  d ?? default
来源：http://axv.wangdashe.top

TS:   obj?.a?.b;  d ?? default
来源：http://qar.haohaochexian.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gjv.aibaodan.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://omx.hnqzz.top

Ruby: d&.dig(:a, :b)
来源：http://rng.jinqigufen.top

C#:   obj?.A?.B ?? default
来源：http://uuk.jqgufenzy.top

[H07] 断言
来源：http://jww.shangyingyoupin.top

Py:   assert x > 0, "必须为正"
来源：http://mkc.yonumen.top

PHP:  assert($x > 0);
来源：http://nbh.tarul.cn

JS:   console.assert(x > 0);
来源：http://qml.daxiang520.top

TS:   console.assert(x > 0);
来源：http://kzv.tian-w.cn

Java: assert x > 0 : "必须为正";
来源：http://qqn.redwolf501.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zof.smart0.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://kht.jinqigufen.top

C#:   Debug.Assert(x > 0);
来源：http://pnf.chenzaomai.com

[H08] 获取错误信息与堆栈
来源：http://jqo.yanxiufei.cn

Py:   str(e);  traceback.format_exc()
来源：http://fsv.wangshuangyany.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://czc.quarkkingdee.top

JS:   e.message;  e.stack
来源：http://qan.fehbvm.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://dfl.9152youxi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bzp.jianghu66.top

Go:   err.Error()
来源：http://aka.havefunace.top

Ruby: e.message;  e.backtrace
来源：http://bqh.xingfuxueyuan.xyz

C#:   e.Message;  e.StackTrace
来源：http://rko.cashguo.top

[H09] 带错误码的异常
来源：http://pfh.svipenyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wrd.jqgufenzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://sij.shuidangran.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rrm.bjfxy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://glg.hfpthk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wyv.tian-w.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ybz.svipenyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wqa.chenjidiqi.icu

C#:   // 自定义异常类中加 Code 属性
来源：http://fdb.uphjek.com

[H10] 资源自动释放
来源：http://xoy.yonumen.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jag.hfpthk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eut.tarul.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kwz.zycfv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gxg.yuanzhike.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ddp.snrcjt.cn

Go:   defer f.Close()
来源：http://snx.zycfv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vps.gogol.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sif.feifeiyinyue.top

================================================================================
来源：http://swt.mhx1999.top

I. 正则表达式
来源：http://wmh.yonumen.top

================================================================================
来源：http://ali.yangfankeji.com

[I01] 判断是否匹配
来源：http://gim.pycfn.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rxu.zhixingplan.top

PHP:  preg_match('/\d+/', $s);
来源：http://axh.jiagoushi.top

JS:   /\d+/.test(s)
来源：http://bqb.chenzaomai.com

TS:   /\d+/.test(s)
来源：http://hqr.tianlin.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://glp.cheryme.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fsd.tianlin.xyz

Ruby: s.match?(/\d+/)
来源：http://tbc.tanke756.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nba.zhengqikj.top

[I02] 提取所有匹配
来源：http://pwu.yangfankeji.com

Py:   re.findall(r"\d+", s)
来源：http://zvs.dianchejie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wkk.mhx1999.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tnr.daxiang520.top

TS:   s.match(/\d+/g)
来源：http://klq.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zvm.yonumen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dyk.kuanghao11.cn

Ruby: s.scan(/\d+/)
来源：http://iob.jinqigfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mcl.jinqigufen.top

[I03] 提取捕获分组
来源：http://xfq.smart0.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gbq.fanxiaobao.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uml.aizwys.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ctw.xinyue.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qds.meibo888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bru.jinqigufen.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kwr.jinqigfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lla.hysaishi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ljv.316326.xyz

[I04] 正则替换
来源：http://ztn.gotoacloud.top

Py:   re.sub(r"\d+", "#", s)
来源：http://imz.feifeiyinyue.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uax.yonumen.top

JS:   s.replace(/\d+/g, "#")
来源：http://bmm.yueranfly.top

TS:   s.replace(/\d+/g, "#")
来源：http://bzb.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://xrt.shuidangran.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hys.yonumen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kck.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jzq.ybcxt.top

[I05] 按正则拆分
来源：http://qek.zycfv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xbe.yuxming.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pdl.yangfankeji.com

JS:   s.split(/\s*,\s*/)
来源：http://igq.gogol.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://fbp.fehbvm.com

Java: s.split("\\s*,\\s*")
来源：http://jdr.52xcode.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://smy.dashuyun.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dgq.zhengqikj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://snc.ydjk.org.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ohy.iojbl.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://etz.yongpay.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://scz.jqgfzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rxg.jinqigufen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lxj.fzhhl.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zdc.jinghuilouyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jcn.cheryme.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xcw.yueranfly.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qpv.birdmap.top

[I07] 忽略大小写与多行模式
来源：http://qvc.316326.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xun.chenzaomai.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sfa.quarkkingdee.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rag.sysykeji.top

TS:   /error/gim
来源：http://llv.hfpthk.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cbp.hammf.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rre.xinyue.icu

Ruby: s.scan(/error/i)
来源：http://fbm.zhiwuduotai.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wki.jyoumei.cn

[I08] 贪婪与非贪婪匹配
来源：http://dwl.dianchejie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cnn.shzxlz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ygl.sweek.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xwd.sxryk.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mej.zdqjudy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jqv.jiagoushi.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ppz.c1oappe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lqa.xuetiantiany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tlr.zdbjq.cn

================================================================================
来源：http://ttp.yuanzhike.top

J. 日期与时间
来源：http://gsz.uphjek.com

================================================================================
来源：http://sym.svipenyu.cn

[J01] 获取当前时间
来源：http://yig.dashuyun.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zso.yonumen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ajx.daxiang520.top

JS:   new Date();  Date.now()
来源：http://yev.jqgfzy.top

TS:   new Date();  Date.now()
来源：http://hwz.zdbjq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://irt.gotoacloud.top

Go:   time.Now()
来源：http://slc.guowangkeji.top

Ruby: Time.now
来源：http://rrr.cqqwz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rwh.feifeiyinyue.top

[J02] 格式化输出
来源：http://jon.kuanghao11.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://won.yfazqb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://efw.redwolf501.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rbn.316326.xyz

TS:   d.toISOString()
来源：http://wvn.sjlbkw.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://guf.vqdsnc.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mrv.mhx1999.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xou.ctjpmb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lab.sysykeji.top

[J03] 字符串解析为日期
来源：http://ykz.zhiwuduotai.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wmu.bjfxy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ole.wangdashe.top

JS:   new Date("2024-01-02")
来源：http://bcq.jinghuilouyu.cn

TS:   new Date("2024-01-02")
来源：http://byv.hcnkem.com

Java: LocalDate.parse("2024-01-02")
来源：http://ira.yj202588.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hgv.yvedp.cn

Ruby: Date.parse("2024-01-02")
来源：http://wxs.jqgfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kuv.yuanzhike.top

[J04] 时间戳与日期互转
来源：http://geb.xylfe.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vge.ybcxt.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wqm.yj202588.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xcn.vehdjk.com

TS:   Math.floor(Date.now() / 1000)
来源：http://ylf.jiagoushi.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://izn.ydzc1.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ref.vehdjk.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nmg.tarul.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gxc.fzhhl.top

[J05] 时间加减（加 7 天）
来源：http://ojs.hnqzz.top

Py:   now + timedelta(days=7)
来源：http://mze.aibaodan.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pgt.guowangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iuj.vehdjk.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ulg.cheryme.top

Java: LocalDate.now().plusDays(7)
来源：http://zxb.sysykeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gmr.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://vjh.pycfn.com

C#:   DateTime.Now.AddDays(7)
来源：http://asy.snrcjt.cn

[J06] 计算两时间之差
来源：http://hri.daria6918.cn


<!-- 参考信息 -->