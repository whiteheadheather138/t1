代发 wailian999

JS:   super.greet();
来源：http://qfj.gaohongyu789.top

TS:   super.greet();
来源：http://vgy.bjfxy.top

Java: super.greet();
来源：http://zlt.gogol.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nbm.sjlbkw.cn

Ruby: super
来源：http://wur.zhoulong.xyz

C#:   base.Greet();
来源：http://naa.zycfv.cn

[G08] 静态方法与属性
来源：http://yjy.svipenyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://thq.jqgufenzy.top

PHP:  public static function f() {}
来源：http://tsn.epnwcf.com

JS:   static f() {}
来源：http://wdx.snrcjt.cn

TS:   static f(): void {}
来源：http://wtl.shanyushiyangtech.top

Java: static void f() {}
来源：http://xje.tian-w.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://liy.jinyuanbaomall.cn

Ruby: def self.f; end
来源：http://yse.xuanzx.com

C#:   public static void F() {}
来源：http://uwq.cdnleiting.top

[G09] 接口 / 抽象类
来源：http://tte.jianghu66.top

Py:   from abc import ABC, abstractmethod
来源：http://iay.fzhhl.top

PHP:  interface Shape { public function area(): float; }
来源：http://ghb.cheryme.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xjy.hammf.cn

TS:   interface Shape { area(): number; }
来源：http://ohm.gzhubu.top

Java: interface Shape { double area(); }
来源：http://gcw.fengsongda.top

Go:   type Shape interface { Area() float64 }
来源：http://som.shangyingyoupin.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zig.jinqigufen.top

C#:   interface IShape { double Area(); }
来源：http://byf.aizwys.cn

[G10] 访问控制
来源：http://rpl.yanxiufei.cn

Py:   约定 _protected / __private（不强制）
来源：http://rai.yj20258.top

PHP:  public / protected / private
来源：http://qhm.cheryme.top

JS:   #private 字段；其余公开
来源：http://veh.jinqigfzy.top

TS:   public / protected / private
来源：http://qdl.chenlongwang.top

Java: public / protected / private / 默认包级
来源：http://ssz.chenlongwang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://oqy.hnxiangtu.top

Ruby: public / protected / private
来源：http://klx.feifeiyinyue.top

C#:   public / protected / private / internal
来源：http://tul.sxryk.cn

[G11] getter / setter
来源：http://sva.smart0.xyz

Py:   @property 与 @x.setter
来源：http://daz.feifeiyinyue.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ops.chenzaomai.com

JS:   get name() { return this._name; }
来源：http://bru.jyoumei.cn

TS:   get name(): string { return this._name; }
来源：http://qxs.0kj1m.cn

Java: public String getName() { return name; }
来源：http://evb.fengsongda.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jff.zhengqikj.top

Ruby: attr_accessor :name
来源：http://rpr.cucudq.cn

C#:   public string Name { get; set; }
来源：http://cqk.jyoumei.cn

[G12] 对象转字符串
来源：http://akw.jinqigfzy.top

Py:   def __str__(self): return self.name
来源：http://mce.vehdjk.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://our.wangshuangyany.cn

JS:   toString() { return this.name; }
来源：http://blr.jqgfzy.top

TS:   toString(): string { return this.name; }
来源：http://nnw.hcnkem.com

Java: @Override public String toString() { return name; }
来源：http://icq.sweek.top

Go:   func (u User) String() string { return u.Name }
来源：http://ckr.zycfv.cn

Ruby: def to_s; @name; end
来源：http://kyg.cucudq.cn

C#:   public override string ToString() => Name;
来源：http://tha.dianchejie.cn

[G13] 判断对象类型
来源：http://oql.c1oappe.top

Py:   isinstance(u, User)
来源：http://yns.zhengqikj.top

PHP:  $u instanceof User
来源：http://ppv.0kj1m.cn

JS:   u instanceof User
来源：http://opc.zdbjq.cn

TS:   u instanceof User
来源：http://njv.mhx1999.top

Java: u instanceof User
来源：http://ltq.xinyue.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://okx.zhijiandao.cn

Ruby: u.is_a?(User)
来源：http://wdc.dashuyun.cn

C#:   u is User
来源：http://deo.epnwcf.com

[G14] 数据类 / record
来源：http://kqu.bjfxy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://drm.xylfe.cn

PHP:  // 用 readonly 属性模拟
来源：http://zvf.epnwcf.com

JS:   // 无内置：普通类或对象字面量
来源：http://dqc.yj20258888.top

TS:   type User = { name: string; age: number };
来源：http://lyd.sjlbkw.cn

Java: record User(String name, int age) {}
来源：http://uls.fanxiaobao.xyz

Go:   type User struct { Name string; Age int }
来源：http://vvt.dianchejie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vep.yonumen.top

C#:   record User(string Name, int Age);
来源：http://iiv.fanxiaobao.xyz

[G15] 枚举
来源：http://xvg.hcnkem.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ibf.yj20258888.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://prp.fengsongda.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hyq.sxryk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eyu.xinyue.icu

Java: enum Color { RED, GREEN }
来源：http://qft.vqdsnc.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mod.yuxming.cn

Ruby: Color = %i[red green].freeze
来源：http://vxq.shangyingyoupin.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wun.tian-w.cn

[G16] 对象转数组 / 字典
来源：http://ura.hesvh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ndw.hfpthk.cn

PHP:  get_object_vars($obj);
来源：http://zpw.quarkkingdee.top

JS:   Object.entries(obj)
来源：http://yke.daria6918.cn

TS:   Object.entries(obj)
来源：http://tmb.guannengcc.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://opn.aizwys.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vcw.xuetiantiany.cn

Ruby: obj.instance_variables
来源：http://gxi.vehdjk.com

C#:   // 用反射或 System.Text.Json
来源：http://eee.nwbrower.top

================================================================================
来源：http://dja.zdqjudy.top

H. 异常与错误处理
来源：http://rma.hesvh.cn

================================================================================
来源：http://wcb.yonumen.top

[H01] try / catch 基础
来源：http://snc.smart0.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lgw.xylfe.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qzx.pycfn.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://etk.xuetiantiany.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gxp.hesvh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://egd.cucudq.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xgg.sufxvd.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fbm.xziqi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wve.xylfe.cn

[H02] finally / ensure 收尾
来源：http://gmr.cucudq.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tix.ehwqpu.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://fqt.nwbrower.top

JS:   try { f(); } finally { cleanup(); }
来源：http://sxz.hammf.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://erb.pycfn.com

Java: try { f(); } finally { cleanup(); }
来源：http://gdm.aizwys.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hmi.gotoacloud.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bna.sufxvd.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ios.xuetiantiany.cn

[H03] 主动抛出异常
来源：http://pdd.shanyushiyangtech.top

Py:   raise ValueError("错误信息")
来源：http://czx.cdnleiting.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dnj.wangdashe.top

JS:   throw new Error("错误信息");
来源：http://clu.hongshengwenyu.top

TS:   throw new Error("错误信息");
来源：http://rhq.andypj.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://jgd.feifeiyinyue.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fzm.zdqjudy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qet.redwolf501.top

C#:   throw new ArgumentException("错误信息");
来源：http://ikq.yj20258888.top

[H04] 自定义异常类型
来源：http://nmf.xuetiantiany.cn

Py:   class MyError(Exception): pass
来源：http://zji.gotoacloud.top

PHP:  class MyError extends RuntimeException {}
来源：http://ycb.jqgfzy.top

JS:   class MyError extends Error {}
来源：http://quw.c1oappe.top

TS:   class MyError extends Error {}
来源：http://xrb.zhijiandao.cn

Java: class MyException extends RuntimeException {}
来源：http://flf.aibaodan.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ehh.smart0.xyz

Ruby: class MyError < StandardError; end
来源：http://hjf.zhongyouzk.top

C#:   class MyException : Exception {}
来源：http://aoy.shangyingyoupin.top

[H05] 捕获特定类型
来源：http://sif.hammf.cn

Py:   except ValueError as e:
来源：http://otw.xziqi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sxh.yanxiufei.cn

JS:   if (e instanceof TypeError) {}
来源：http://cnt.sweek.top

TS:   if (e instanceof TypeError) {}
来源：http://opp.gaohongyu789.top

Java: catch (IOException | SQLException e) {}
来源：http://mvt.hysaishi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lih.xziqi.cn

Ruby: rescue ArgumentError => e
来源：http://cmi.hnxiangtu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tzy.pengpengdd.cyou

[H06] 可选值 / 空值安全访问
来源：http://qli.gzhubu.top

Py:   value = d.get("k") or default
来源：http://fwn.epnwcf.com

PHP:  $v = $d["k"] ?? null;
来源：http://amn.ydjk.org.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pcv.c1oappe.top

TS:   obj?.a?.b;  d ?? default
来源：http://uiw.ehwqpu.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nrx.vqdsnc.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lug.guowangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://cic.fehbvm.com

C#:   obj?.A?.B ?? default
来源：http://mvh.guowangkeji.top

[H07] 断言
来源：http://fuq.xziqi.cn

Py:   assert x > 0, "必须为正"
来源：http://lqa.nwbrower.top

PHP:  assert($x > 0);
来源：http://vit.ywan-chungtsiang.top

JS:   console.assert(x > 0);
来源：http://viy.hfpthk.cn

TS:   console.assert(x > 0);
来源：http://whj.hesvh.cn

Java: assert x > 0 : "必须为正";
来源：http://zuv.ehwqpu.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uyd.vehdjk.com

Ruby: raise "必须为正" unless x > 0
来源：http://axc.cashguo.top

C#:   Debug.Assert(x > 0);
来源：http://lnt.fengsongda.top

[H08] 获取错误信息与堆栈
来源：http://roo.vehdjk.com

Py:   str(e);  traceback.format_exc()
来源：http://fyz.yj20258888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qfh.ydzc1.top

JS:   e.message;  e.stack
来源：http://zso.jinyuanbaomall.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://uhg.zhongyouzk.top

Java: e.getMessage();  e.printStackTrace()
来源：http://skn.guowangkeji.top

Go:   err.Error()
来源：http://kbm.jqgufenzy.top

Ruby: e.message;  e.backtrace
来源：http://rld.hcnkem.com

C#:   e.Message;  e.StackTrace
来源：http://kpq.jinyuanbaomall.cn

[H09] 带错误码的异常
来源：http://nhz.yvedp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hvr.quarkkingdee.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://thw.smart0.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yfk.havefunace.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://udl.fehbvm.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ckx.fanxiaobao.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jkc.pycfn.com

Ruby: raise MyError.new("fail", 500)
来源：http://cgc.yj20258.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zpb.yanxiufei.cn

[H10] 资源自动释放
来源：http://zdk.fengsongda.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://zai.9152youxi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fza.jinqigufen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bvx.hcnkem.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://joi.zhongyouzk.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nlt.jiagoushi.top

Go:   defer f.Close()
来源：http://qma.sweek.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iur.yj20258888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zuy.shangyingyoupin.top

================================================================================
来源：http://fhj.iojbl.cn

I. 正则表达式
来源：http://kgi.hnqzz.top

================================================================================
来源：http://jlo.xinyue.icu

[I01] 判断是否匹配
来源：http://lqu.cdnleiting.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qcs.yongpay.top

PHP:  preg_match('/\d+/', $s);
来源：http://imi.wangshuangyany.cn

JS:   /\d+/.test(s)
来源：http://bay.jyoumei.cn

TS:   /\d+/.test(s)
来源：http://tve.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cnt.hcnkem.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mzm.jinyuanbaomall.cn

Ruby: s.match?(/\d+/)
来源：http://orw.nanxinkj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vcq.pycfn.com

[I02] 提取所有匹配
来源：http://arh.epnwcf.com

Py:   re.findall(r"\d+", s)
来源：http://gsk.xingfuxueyuan.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cnm.hongshengwenyu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rfk.gzhubu.top

TS:   s.match(/\d+/g)
来源：http://tyb.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ncv.xinyue.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jsj.meibo888.top

Ruby: s.scan(/\d+/)
来源：http://ink.yj20258.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ymk.gotoacloud.top

[I03] 提取捕获分组
来源：http://jzh.yvedp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gff.yuanzhike.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jxa.chenjidiqi.icu

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://icb.aibaodan.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ecl.yj20258888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lhk.hammf.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vwk.cheryme.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ynn.mhx1999.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zrx.bbcook.cn

[I04] 正则替换
来源：http://cnf.jqgfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hnu.xuanzx.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gew.pengpengdd.cyou

JS:   s.replace(/\d+/g, "#")
来源：http://wpc.jinyuanbaomall.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zoj.shuidangran.top

Java: s.replaceAll("\\d+", "#")
来源：http://lmg.ctjpmb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://kiv.redwolf501.top

Ruby: s.gsub(/\d+/, "#")
来源：http://sty.smart0.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uhp.cheryme.top

[I05] 按正则拆分
来源：http://gyu.sweek.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bys.hongshengwenyu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tea.hnxiangtu.top

JS:   s.split(/\s*,\s*/)
来源：http://kjj.xinyue.icu

TS:   s.split(/\s*,\s*/)
来源：http://gcs.zdbjq.cn

Java: s.split("\\s*,\\s*")
来源：http://dux.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hqa.hnqzz.top

Ruby: s.split(/\s*,\s*/)
来源：http://opa.chenlongwang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qky.vqdsnc.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ffb.vehdjk.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://adm.zhengqikj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rte.shangyingyoupin.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xvr.zdbjq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://clw.fzhhl.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lqr.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lnm.9152youxi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://npt.mhx1999.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wme.uphjek.com

[I07] 忽略大小写与多行模式
来源：http://fqj.yangfankeji.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oad.zhengqikj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oke.hongshengwenyu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cvv.shzxlz.cn

TS:   /error/gim
来源：http://jrv.gogol.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fpv.haohaochexian.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rkr.ctjpmb.com

Ruby: s.scan(/error/i)
来源：http://kau.bbcook.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pmr.xylfe.cn

[I08] 贪婪与非贪婪匹配
来源：http://kiv.shzxlz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ayh.yueranfly.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://drx.fehbvm.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fhw.chenjidiqi.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ffg.nwbrower.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://eia.ivvv.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://udq.9152youxi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vkp.gogol.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lhu.sufxvd.cn

================================================================================
来源：http://vdr.iojbl.cn

J. 日期与时间
来源：http://flg.zhiwuduotai.top

================================================================================
来源：http://cel.sjlbkw.cn

[J01] 获取当前时间
来源：http://idm.zhoulong.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://kmk.yuanzhike.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blw.cucudq.cn

JS:   new Date();  Date.now()
来源：http://vax.jinqigufen.top

TS:   new Date();  Date.now()
来源：http://vff.chenzaomai.com

Java: LocalDateTime.now();  Instant.now()
来源：http://efd.tian-w.cn

Go:   time.Now()
来源：http://sff.birdmap.top

Ruby: Time.now
来源：http://lbv.jinghuilouyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://moo.hnqzz.top

[J02] 格式化输出
来源：http://bqz.wangdashe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wgn.cqqwz.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yvx.jinqigufen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://osv.tanke756.top

TS:   d.toISOString()
来源：http://uyn.0kj1m.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bsq.gaohongyu789.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xbv.epnwcf.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oaj.chenlongwang.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zje.xinyue.icu

[J03] 字符串解析为日期
来源：http://uqt.9152youxi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bxg.mhx1999.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xvm.cqqwz.cn

JS:   new Date("2024-01-02")
来源：http://ngt.pengpengdd.cyou

TS:   new Date("2024-01-02")
来源：http://qhu.ywan-chungtsiang.top

Java: LocalDate.parse("2024-01-02")
来源：http://oxe.epnwcf.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gsf.xylfe.cn

Ruby: Date.parse("2024-01-02")
来源：http://udx.jqgufenzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qom.shanyushiyangtech.top

[J04] 时间戳与日期互转
来源：http://zzd.yonumen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://adu.hongshengwenyu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ews.meibo888.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uws.yonumen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://awx.yanxiufei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hxm.ehwqpu.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cjp.kuanghao11.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hqc.redwolf501.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ehg.epnwcf.com

[J05] 时间加减（加 7 天）
来源：http://yvt.yfazqb.com

Py:   now + timedelta(days=7)
来源：http://zfi.havefunace.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rtg.sufxvd.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bqu.hfpthk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yij.dianchejie.cn

Java: LocalDate.now().plusDays(7)
来源：http://lnz.redwolf501.top


<!-- 参考信息 -->