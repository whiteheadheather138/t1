代发 wailian999

Ruby: super
来源：http://kfc.smart0.xyz

C#:   base.Greet();
来源：http://ujb.0kj1m.cn

[G08] 静态方法与属性
来源：http://gfx.ydjk.org.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gvl.zhixingplan.top

PHP:  public static function f() {}
来源：http://hfn.ywan-chungtsiang.top

JS:   static f() {}
来源：http://wqu.epnwcf.com

TS:   static f(): void {}
来源：http://rsn.ppjwa.cn

Java: static void f() {}
来源：http://vra.pycfn.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://qmw.sweek.top

Ruby: def self.f; end
来源：http://xpq.xinyue.icu

C#:   public static void F() {}
来源：http://sgv.shzxlz.cn

[G09] 接口 / 抽象类
来源：http://tgu.gogol.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://ujv.bjfxy.top

PHP:  interface Shape { public function area(): float; }
来源：http://hiv.ivvv.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tnh.cashguo.top

TS:   interface Shape { area(): number; }
来源：http://xxf.yj20258.top

Java: interface Shape { double area(); }
来源：http://xnc.hongshengwenyu.top

Go:   type Shape interface { Area() float64 }
来源：http://kzh.fehbvm.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nff.kuanghao11.cn

C#:   interface IShape { double Area(); }
来源：http://lnl.cucudq.cn

[G10] 访问控制
来源：http://jgp.fanxiaobao.xyz

Py:   约定 _protected / __private（不强制）
来源：http://kku.chenlongwang.top

PHP:  public / protected / private
来源：http://pbv.c1oappe.top

JS:   #private 字段；其余公开
来源：http://ifu.fehbvm.com

TS:   public / protected / private
来源：http://uqs.zhijiandao.cn

Java: public / protected / private / 默认包级
来源：http://pdh.yuxming.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vgw.ydzc1.top

Ruby: public / protected / private
来源：http://bwc.cdnleiting.top

C#:   public / protected / private / internal
来源：http://rsz.hcnkem.com

[G11] getter / setter
来源：http://oek.jinqigfzy.top

Py:   @property 与 @x.setter
来源：http://cop.ywan-chungtsiang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qcy.zhoulong.xyz

JS:   get name() { return this._name; }
来源：http://zgm.yueranfly.top

TS:   get name(): string { return this._name; }
来源：http://zcw.cucudq.cn

Java: public String getName() { return name; }
来源：http://gvr.yongpay.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://sci.jiagoushi.top

Ruby: attr_accessor :name
来源：http://qzq.xingfuxueyuan.xyz

C#:   public string Name { get; set; }
来源：http://jfs.dianchejie.cn

[G12] 对象转字符串
来源：http://fmm.gogol.net.cn

Py:   def __str__(self): return self.name
来源：http://zzn.gaohongyu789.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xcv.zhengqikj.top

JS:   toString() { return this.name; }
来源：http://swn.hfpthk.cn

TS:   toString(): string { return this.name; }
来源：http://nlm.jyoumei.cn

Java: @Override public String toString() { return name; }
来源：http://fzq.9152youxi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rkx.cheryme.top

Ruby: def to_s; @name; end
来源：http://rlb.xziqi.cn

C#:   public override string ToString() => Name;
来源：http://gxz.daria6918.cn

[G13] 判断对象类型
来源：http://jta.cdnleiting.top

Py:   isinstance(u, User)
来源：http://wfa.zhoulong.xyz

PHP:  $u instanceof User
来源：http://wwj.tarul.cn

JS:   u instanceof User
来源：http://sfi.mhx1999.top

TS:   u instanceof User
来源：http://pxp.ppjwa.cn

Java: u instanceof User
来源：http://kqu.guowangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ici.redwolf501.top

Ruby: u.is_a?(User)
来源：http://diq.chenlongwang.top

C#:   u is User
来源：http://rxf.jyoumei.cn

[G14] 数据类 / record
来源：http://pls.nanxinkj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cqv.chenzaomai.com

PHP:  // 用 readonly 属性模拟
来源：http://spl.fanxiaobao.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://wit.nwbrower.top

TS:   type User = { name: string; age: number };
来源：http://oyg.ywan-chungtsiang.top

Java: record User(String name, int age) {}
来源：http://tuv.chenjidiqi.icu

Go:   type User struct { Name string; Age int }
来源：http://vul.yanxiufei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://won.tianlin.xyz

C#:   record User(string Name, int Age);
来源：http://zpl.hesvh.cn

[G15] 枚举
来源：http://qqc.pycfn.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xwa.epnwcf.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://los.shuidangran.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dnr.shzxlz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mdd.jyoumei.cn

Java: enum Color { RED, GREEN }
来源：http://daw.bjfxy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://icl.zycfv.cn

Ruby: Color = %i[red green].freeze
来源：http://tfd.wangshuangyany.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jwl.fzhhl.top

[G16] 对象转数组 / 字典
来源：http://wys.xinyue.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nyj.vehdjk.com

PHP:  get_object_vars($obj);
来源：http://lyh.uphjek.com

JS:   Object.entries(obj)
来源：http://vsc.redwolf501.top

TS:   Object.entries(obj)
来源：http://qdt.yongpay.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sqj.wangshuangyany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://syi.wangdashe.top

Ruby: obj.instance_variables
来源：http://hpm.cashguo.top

C#:   // 用反射或 System.Text.Json
来源：http://ten.jinqigfzy.top

================================================================================
来源：http://fqm.cheryme.top

H. 异常与错误处理
来源：http://tqz.zhoulong.xyz

================================================================================
来源：http://qav.zdbjq.cn

[H01] try / catch 基础
来源：http://jki.fengsongda.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jwx.zhixingplan.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rag.jianghu66.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dzy.tarul.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nxb.shanyushiyangtech.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://esi.svipenyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://brg.haohaochexian.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://azy.yfazqb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hst.bbcook.cn

[H02] finally / ensure 收尾
来源：http://nmp.bbcook.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rbt.yj20258.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ecx.ywan-chungtsiang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vje.jlsjyb.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dpy.hnxiangtu.top

Java: try { f(); } finally { cleanup(); }
来源：http://gat.wangdashe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ipq.hnxiangtu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ulq.pengpengdd.cyou

C#:   try { F(); } finally { Cleanup(); }
来源：http://phw.haohaochexian.top

[H03] 主动抛出异常
来源：http://zdn.fehbvm.com

Py:   raise ValueError("错误信息")
来源：http://tie.pengpengdd.cyou

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://iej.zhoulong.xyz

JS:   throw new Error("错误信息");
来源：http://uvc.quarkkingdee.top

TS:   throw new Error("错误信息");
来源：http://eff.chenlongwang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://obg.shanyushiyangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wte.9152youxi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zhb.zhongyouzk.top

C#:   throw new ArgumentException("错误信息");
来源：http://lkn.jqgufenzy.top

[H04] 自定义异常类型
来源：http://vpg.zhijiandao.cn

Py:   class MyError(Exception): pass
来源：http://xdy.zycfv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fqu.xinyue.icu

JS:   class MyError extends Error {}
来源：http://czy.jqgfzy.top

TS:   class MyError extends Error {}
来源：http://qgm.yueranfly.top

Java: class MyException extends RuntimeException {}
来源：http://ees.daxiang520.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eak.hcnkem.com

Ruby: class MyError < StandardError; end
来源：http://fbf.yj20258.top

C#:   class MyException : Exception {}
来源：http://okt.xingfuxueyuan.xyz

[H05] 捕获特定类型
来源：http://bku.ydjk.org.cn

Py:   except ValueError as e:
来源：http://bmi.zycfv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nvn.hfpthk.cn

JS:   if (e instanceof TypeError) {}
来源：http://kmo.meibo888.top

TS:   if (e instanceof TypeError) {}
来源：http://ttf.jianghu66.top

Java: catch (IOException | SQLException e) {}
来源：http://xfp.wangdashe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fqt.jyoumei.cn

Ruby: rescue ArgumentError => e
来源：http://uvf.nanxinkj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gvj.yangfankeji.com

[H06] 可选值 / 空值安全访问
来源：http://iju.andypj.xyz

Py:   value = d.get("k") or default
来源：http://rba.9152youxi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://uxn.tianlin.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://dos.yueranfly.top

TS:   obj?.a?.b;  d ?? default
来源：http://nti.uphjek.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mca.hfpthk.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vig.nanxinkj.top

Ruby: d&.dig(:a, :b)
来源：http://vqq.zdbjq.cn

C#:   obj?.A?.B ?? default
来源：http://bpr.dianchejie.cn

[H07] 断言
来源：http://aks.cucudq.cn

Py:   assert x > 0, "必须为正"
来源：http://kpw.316326.xyz

PHP:  assert($x > 0);
来源：http://auu.jianghu66.top

JS:   console.assert(x > 0);
来源：http://qwg.meibo888.top

TS:   console.assert(x > 0);
来源：http://snb.feifeiyinyue.top

Java: assert x > 0 : "必须为正";
来源：http://dtq.sweek.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yir.zycfv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bcz.zhijiandao.cn

C#:   Debug.Assert(x > 0);
来源：http://zvv.zycfv.cn

[H08] 获取错误信息与堆栈
来源：http://lei.ywan-chungtsiang.top

Py:   str(e);  traceback.format_exc()
来源：http://fqt.hysaishi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://edx.xinyue.icu

JS:   e.message;  e.stack
来源：http://azs.jianghu66.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xep.cucudq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://edj.jqgufenzy.top

Go:   err.Error()
来源：http://pav.jlsjyb.cn

Ruby: e.message;  e.backtrace
来源：http://szw.ydzc1.top

C#:   e.Message;  e.StackTrace
来源：http://gyg.ppjwa.cn

[H09] 带错误码的异常
来源：http://wvf.vehdjk.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xov.xinyue.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://wus.sysykeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zri.jlsjyb.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yzi.dashuyun.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iyq.ehwqpu.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zkb.chenlongwang.top

Ruby: raise MyError.new("fail", 500)
来源：http://odw.hcnkem.com

C#:   // 自定义异常类中加 Code 属性
来源：http://oxa.guannengcc.top

[H10] 资源自动释放
来源：http://grv.wangshuangyany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ksm.zdbjq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vmp.zhaomingkeji.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ang.zhoulong.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sml.zhaomingkeji.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vwn.shanyushiyangtech.top

Go:   defer f.Close()
来源：http://wbv.yueranfly.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ijb.ydzc1.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vil.nwbrower.top

================================================================================
来源：http://fnr.svipenyu.cn

I. 正则表达式
来源：http://ysl.nanxinkj.top

================================================================================
来源：http://ept.yfazqb.com

[I01] 判断是否匹配
来源：http://wva.nanxinkj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nyt.zhiwuduotai.top

PHP:  preg_match('/\d+/', $s);
来源：http://scj.iojbl.cn

JS:   /\d+/.test(s)
来源：http://fot.tianlin.xyz

TS:   /\d+/.test(s)
来源：http://okx.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://goy.xylfe.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zbk.zdbjq.cn

Ruby: s.match?(/\d+/)
来源：http://imv.ywan-chungtsiang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://elf.yuxming.cn

[I02] 提取所有匹配
来源：http://ckp.gotoacloud.top

Py:   re.findall(r"\d+", s)
来源：http://vil.sufxvd.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dmr.yangfankeji.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zlh.nanxinkj.top

TS:   s.match(/\d+/g)
来源：http://nnf.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ich.wangdashe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rmy.hnxiangtu.top

Ruby: s.scan(/\d+/)
来源：http://gat.hfpthk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fyf.vehdjk.com

[I03] 提取捕获分组
来源：http://kcb.snrcjt.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jxb.zhengqikj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wzt.tian-w.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://njq.birdmap.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rba.shangyingyoupin.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cfv.epnwcf.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sxv.dashuyun.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zep.tian-w.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://irv.shzxlz.cn

[I04] 正则替换
来源：http://zfs.chenlongwang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qte.kuanghao11.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uhc.mhx1999.top

JS:   s.replace(/\d+/g, "#")
来源：http://hmy.guannengcc.top

TS:   s.replace(/\d+/g, "#")
来源：http://leo.hysaishi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fwt.daria6918.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ufe.ybcxt.top

Ruby: s.gsub(/\d+/, "#")
来源：http://cyd.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vcb.xuanzx.com

[I05] 按正则拆分
来源：http://qtg.xylfe.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bjk.shzxlz.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lqo.tianlin.xyz

JS:   s.split(/\s*,\s*/)
来源：http://shh.xuanzx.com

TS:   s.split(/\s*,\s*/)
来源：http://dkv.yj20258888.top

Java: s.split("\\s*,\\s*")
来源：http://qvd.yj202588.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ymw.havefunace.top

Ruby: s.split(/\s*,\s*/)
来源：http://oqq.redwolf501.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ifd.shuidangran.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fqi.yuxming.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kas.ivvv.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nhb.zhaomingkeji.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ujv.aibaodan.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aoa.chenlongwang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hdx.zhiwuduotai.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ehu.cheryme.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://osr.zhijiandao.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mig.hfpthk.cn

[I07] 忽略大小写与多行模式
来源：http://yum.yfazqb.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hug.cheryme.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iim.aizwys.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xld.shuidangran.top

TS:   /error/gim
来源：http://apz.tianlin.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jlw.sysykeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://klq.zhongyouzk.top

Ruby: s.scan(/error/i)
来源：http://zls.ivvv.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nfk.zhiwuduotai.top

[I08] 贪婪与非贪婪匹配
来源：http://syr.9152youxi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://chk.jianghu66.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hxa.gaohongyu789.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qlb.hammf.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nza.52xcode.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://flh.shanyushiyangtech.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sve.guowangkeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uqs.hysaishi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mpw.uphjek.com

================================================================================
来源：http://xrn.feifeiyinyue.top

J. 日期与时间
来源：http://sno.yonumen.top

================================================================================
来源：http://xlm.tarul.cn

[J01] 获取当前时间
来源：http://osc.gaohongyu789.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ucc.hnxiangtu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fiu.xuanzx.com

JS:   new Date();  Date.now()
来源：http://kvf.daxiang520.top

TS:   new Date();  Date.now()
来源：http://qki.chenzaomai.com

Java: LocalDateTime.now();  Instant.now()
来源：http://atv.hnqzz.top

Go:   time.Now()
来源：http://baw.cucudq.cn

Ruby: Time.now
来源：http://lfi.xziqi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lql.daria6918.cn

[J02] 格式化输出
来源：http://nmd.yangfankeji.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wct.cucudq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://onq.haohaochexian.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mrn.fanxiaobao.xyz

TS:   d.toISOString()
来源：http://eng.dashuyun.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xkc.jinqigfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yty.gogol.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ejd.pycfn.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://utg.fehbvm.com

[J03] 字符串解析为日期
来源：http://cze.chenjidiqi.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kad.jyoumei.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ktc.0kj1m.cn

JS:   new Date("2024-01-02")
来源：http://gji.yj20258.top

TS:   new Date("2024-01-02")
来源：http://qqh.bbcook.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mgt.haohaochexian.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rim.mhx1999.top

Ruby: Date.parse("2024-01-02")
来源：http://bsj.fehbvm.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://djs.zhixingplan.top

[J04] 时间戳与日期互转
来源：http://zoe.dashuyun.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qam.sjlbkw.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mkc.nanxuanxn.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fsu.316326.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://mkw.cheryme.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://asx.yfazqb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wpy.ydzc1.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ljg.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xhg.shzxlz.cn

[J05] 时间加减（加 7 天）
来源：http://jln.jinghuilouyu.cn

Py:   now + timedelta(days=7)
来源：http://vfj.jlsjyb.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wlm.ybcxt.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zox.chenlongwang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zsi.ywan-chungtsiang.top

Java: LocalDate.now().plusDays(7)
来源：http://fhi.zycfv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fna.quarkkingdee.top

Ruby: Time.now + 7 * 86400
来源：http://pue.kuanghao11.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lcl.hnqzz.top

[J06] 计算两时间之差
来源：http://gwp.wangdashe.top


<!-- 参考信息 -->