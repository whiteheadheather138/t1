代发 wailian999

PHP:  public static function f() {}
来源：http://bdk.hywenlv.cn

JS:   static f() {}
来源：http://tnq.gotoacloud.top

TS:   static f(): void {}
来源：http://bmu.yongpay.top

Java: static void f() {}
来源：http://eyl.xuetiantiany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wsu.vqdsnc.cn

Ruby: def self.f; end
来源：http://cqj.0kj1m.cn

C#:   public static void F() {}
来源：http://bzo.pycfn.com

[G09] 接口 / 抽象类
来源：http://kjc.52xcode.cn

Py:   from abc import ABC, abstractmethod
来源：http://xtw.fehbvm.com

PHP:  interface Shape { public function area(): float; }
来源：http://qcd.jinqigufen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ire.hammf.cn

TS:   interface Shape { area(): number; }
来源：http://fug.yvedp.cn

Java: interface Shape { double area(); }
来源：http://epu.wangdashe.top

Go:   type Shape interface { Area() float64 }
来源：http://sfs.ehwqpu.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ltt.ydjk.org.cn

C#:   interface IShape { double Area(); }
来源：http://uos.hnxiangtu.top

[G10] 访问控制
来源：http://zai.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://hzr.haohaochexian.top

PHP:  public / protected / private
来源：http://udv.smart0.xyz

JS:   #private 字段；其余公开
来源：http://ipy.shanyushiyangtech.top

TS:   public / protected / private
来源：http://tmp.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://ccu.jianghu66.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://yqm.wangdashe.top

Ruby: public / protected / private
来源：http://tnw.hongshengwenyu.top

C#:   public / protected / private / internal
来源：http://ody.sufxvd.cn

[G11] getter / setter
来源：http://haz.ehwqpu.com

Py:   @property 与 @x.setter
来源：http://kqg.zhiwuduotai.top

PHP:  public function getName(): string { return $this->name; }
来源：http://lhi.uphjek.com

JS:   get name() { return this._name; }
来源：http://yrf.smart0.xyz

TS:   get name(): string { return this._name; }
来源：http://fik.quarkkingdee.top

Java: public String getName() { return name; }
来源：http://ong.jiagoushi.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jtg.snrcjt.cn

Ruby: attr_accessor :name
来源：http://rqv.nwbrower.top

C#:   public string Name { get; set; }
来源：http://kdx.zhixingplan.top

[G12] 对象转字符串
来源：http://pgl.fktsv.cn

Py:   def __str__(self): return self.name
来源：http://xcx.sxryk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://eln.dashuyun.cn

JS:   toString() { return this.name; }
来源：http://uhz.daria6918.cn

TS:   toString(): string { return this.name; }
来源：http://sbk.xingfuxueyuan.xyz

Java: @Override public String toString() { return name; }
来源：http://fmq.9152youxi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lxa.cucudq.cn

Ruby: def to_s; @name; end
来源：http://xyw.xinyue.icu

C#:   public override string ToString() => Name;
来源：http://vwd.cqqwz.cn

[G13] 判断对象类型
来源：http://lys.xingfuxueyuan.xyz

Py:   isinstance(u, User)
来源：http://gab.andypj.xyz

PHP:  $u instanceof User
来源：http://rwj.sxryk.cn

JS:   u instanceof User
来源：http://tuf.bbcook.cn

TS:   u instanceof User
来源：http://ntd.hesvh.cn

Java: u instanceof User
来源：http://zfo.tarul.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qyx.ydzc1.top

Ruby: u.is_a?(User)
来源：http://uve.cucudq.cn

C#:   u is User
来源：http://hwl.zdqjudy.top

[G14] 数据类 / record
来源：http://qpu.xingfuxueyuan.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kja.cashguo.top

PHP:  // 用 readonly 属性模拟
来源：http://cgy.pycfn.com

JS:   // 无内置：普通类或对象字面量
来源：http://ytk.jiagoushi.top

TS:   type User = { name: string; age: number };
来源：http://psa.gotoacloud.top

Java: record User(String name, int age) {}
来源：http://hqk.ehwqpu.com

Go:   type User struct { Name string; Age int }
来源：http://fse.kuanghao11.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://orx.chenjidiqi.icu

C#:   record User(string Name, int Age);
来源：http://tth.316326.xyz

[G15] 枚举
来源：http://wwi.shuidangran.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zfc.yj202588.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://fdg.gotoacloud.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ijf.pycfn.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qdq.yuxming.cn

Java: enum Color { RED, GREEN }
来源：http://kqj.shzxlz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wsi.chenlongwang.top

Ruby: Color = %i[red green].freeze
来源：http://mkp.chenlongwang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://luk.daria6918.cn

[G16] 对象转数组 / 字典
来源：http://gmr.xziqi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ejq.xylfe.cn

PHP:  get_object_vars($obj);
来源：http://eif.gaohongyu789.top

JS:   Object.entries(obj)
来源：http://poi.hammf.cn

TS:   Object.entries(obj)
来源：http://jet.aibaodan.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zrn.hnqzz.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vze.jinghuilouyu.cn

Ruby: obj.instance_variables
来源：http://agk.jyoumei.cn

C#:   // 用反射或 System.Text.Json
来源：http://fwd.zdqjudy.top

================================================================================
来源：http://fvk.yvedp.cn

H. 异常与错误处理
来源：http://ptc.fzhhl.top

================================================================================
来源：http://zgk.ehwqpu.com

[H01] try / catch 基础
来源：http://pxm.hnqzz.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ijp.kuanghao11.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qwi.sufxvd.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pua.zhixingplan.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://thg.chenzaomai.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ugx.zhaomingkeji.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zni.dianchejie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pyy.hnqzz.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cnh.cheryme.top

[H02] finally / ensure 收尾
来源：http://xbt.jinqigfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://wey.shzxlz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lib.pengpengdd.cyou

JS:   try { f(); } finally { cleanup(); }
来源：http://taj.pycfn.com

TS:   try { f(); } finally { cleanup(); }
来源：http://our.zycfv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zzz.ydzc1.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ytw.iojbl.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dod.zdqjudy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://bke.c1oappe.top

[H03] 主动抛出异常
来源：http://bnk.hnqzz.top

Py:   raise ValueError("错误信息")
来源：http://ccu.yuxming.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ubj.havefunace.top

JS:   throw new Error("错误信息");
来源：http://evi.yongpay.top

TS:   throw new Error("错误信息");
来源：http://hcg.jianghu66.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://cgx.snrcjt.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://srq.quarkkingdee.top

Ruby: raise ArgumentError, "错误信息"
来源：http://wcj.hcnkem.com

C#:   throw new ArgumentException("错误信息");
来源：http://fuk.yvedp.cn

[H04] 自定义异常类型
来源：http://ett.jlsjyb.cn

Py:   class MyError(Exception): pass
来源：http://opz.yj202588.top

PHP:  class MyError extends RuntimeException {}
来源：http://eat.hywenlv.cn

JS:   class MyError extends Error {}
来源：http://jry.snrcjt.cn

TS:   class MyError extends Error {}
来源：http://opn.guannengcc.top

Java: class MyException extends RuntimeException {}
来源：http://fxh.ppjwa.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oui.shuidangran.top

Ruby: class MyError < StandardError; end
来源：http://jbv.ehwqpu.com

C#:   class MyException : Exception {}
来源：http://qqu.redwolf501.top

[H05] 捕获特定类型
来源：http://ksv.ywan-chungtsiang.top

Py:   except ValueError as e:
来源：http://wrm.yj20258.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://txt.jlsjyb.cn

JS:   if (e instanceof TypeError) {}
来源：http://ros.hnqzz.top

TS:   if (e instanceof TypeError) {}
来源：http://dij.aibaodan.cn

Java: catch (IOException | SQLException e) {}
来源：http://wtt.quarkkingdee.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wql.hysaishi.cn

Ruby: rescue ArgumentError => e
来源：http://ras.yfazqb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kzw.ydzc1.top

[H06] 可选值 / 空值安全访问
来源：http://fir.shzxlz.cn

Py:   value = d.get("k") or default
来源：http://hxy.iojbl.cn

PHP:  $v = $d["k"] ?? null;
来源：http://anq.zhijiandao.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ccq.tian-w.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lkm.xuanzx.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rpu.vqdsnc.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xuf.aizwys.cn

Ruby: d&.dig(:a, :b)
来源：http://yri.hywenlv.cn

C#:   obj?.A?.B ?? default
来源：http://eev.zdbjq.cn

[H07] 断言
来源：http://uee.ivvv.top

Py:   assert x > 0, "必须为正"
来源：http://mmy.zdbjq.cn

PHP:  assert($x > 0);
来源：http://feb.zhaomingkeji.xyz

JS:   console.assert(x > 0);
来源：http://ykn.vqdsnc.cn

TS:   console.assert(x > 0);
来源：http://zbs.shanyushiyangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://zvl.yangfankeji.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pax.chenlongwang.top

Ruby: raise "必须为正" unless x > 0
来源：http://kdm.tanke756.top

C#:   Debug.Assert(x > 0);
来源：http://tmx.zdbjq.cn

[H08] 获取错误信息与堆栈
来源：http://kbk.dashuyun.cn

Py:   str(e);  traceback.format_exc()
来源：http://ewr.jlsjyb.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mls.sufxvd.cn

JS:   e.message;  e.stack
来源：http://kzj.smart0.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://hlu.ctjpmb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://zhk.yueranfly.top

Go:   err.Error()
来源：http://xot.nanxinkj.top

Ruby: e.message;  e.backtrace
来源：http://bnl.hongshengwenyu.top

C#:   e.Message;  e.StackTrace
来源：http://gey.jianghu66.top

[H09] 带错误码的异常
来源：http://cgd.hfpthk.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pet.yangfankeji.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://jfm.hnxiangtu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hly.ehwqpu.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bhb.jinqigfzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wff.smart0.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bxs.uphjek.com

Ruby: raise MyError.new("fail", 500)
来源：http://yjh.guannengcc.top

C#:   // 自定义异常类中加 Code 属性
来源：http://yjs.ctjpmb.com

[H10] 资源自动释放
来源：http://cbk.iojbl.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://khq.ppjwa.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lll.cashguo.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ivb.bbcook.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uiz.sysykeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wlx.nanxuanxn.top

Go:   defer f.Close()
来源：http://nyt.sysykeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jcg.hnqzz.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cvj.xuanzx.com

================================================================================
来源：http://rxv.smart0.xyz

I. 正则表达式
来源：http://wqr.zhoulong.xyz

================================================================================
来源：http://eve.chenjidiqi.icu

[I01] 判断是否匹配
来源：http://svr.9152youxi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uti.hywenlv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lly.daxiang520.top

JS:   /\d+/.test(s)
来源：http://yss.shanyushiyangtech.top

TS:   /\d+/.test(s)
来源：http://eok.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nxz.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nyg.ehwqpu.com

Ruby: s.match?(/\d+/)
来源：http://smq.zhixingplan.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zzn.vehdjk.com

[I02] 提取所有匹配
来源：http://yab.jlsjyb.cn

Py:   re.findall(r"\d+", s)
来源：http://ivy.snrcjt.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yyc.gotoacloud.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hkz.yueranfly.top

TS:   s.match(/\d+/g)
来源：http://qai.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://eti.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sez.sweek.top

Ruby: s.scan(/\d+/)
来源：http://vmp.xuanzx.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pvu.fengsongda.top

[I03] 提取捕获分组
来源：http://oqg.daria6918.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://usk.zdqjudy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gom.redwolf501.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nra.hnxiangtu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fsb.jinghuilouyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mfy.tianlin.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://erq.gzhubu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qfk.sjlbkw.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kgl.chenjidiqi.icu

[I04] 正则替换
来源：http://hvg.zhengqikj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://grp.mhx1999.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dmp.jyoumei.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nje.9152youxi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://drx.gaohongyu789.top

Java: s.replaceAll("\\d+", "#")
来源：http://owp.dashuyun.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gsq.xuanzx.com

Ruby: s.gsub(/\d+/, "#")
来源：http://ahp.xuanzx.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mew.svipenyu.cn

[I05] 按正则拆分
来源：http://bkf.hysaishi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sdj.hesvh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jxd.xinyue.icu

JS:   s.split(/\s*,\s*/)
来源：http://tba.shangyingyoupin.top

TS:   s.split(/\s*,\s*/)
来源：http://ota.zdqjudy.top

Java: s.split("\\s*,\\s*")
来源：http://jvh.dashuyun.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iko.yj20258888.top

Ruby: s.split(/\s*,\s*/)
来源：http://uzh.yongpay.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ygn.shanyushiyangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rnm.xinyue.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xqy.gotoacloud.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vce.feifeiyinyue.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mmq.zhengqikj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zfc.ybcxt.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nqj.xuetiantiany.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dms.hnqzz.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nll.yj202588.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tfx.feifeiyinyue.top

[I07] 忽略大小写与多行模式
来源：http://byq.sxryk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://drj.sxryk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ltj.jyoumei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oiy.gotoacloud.top

TS:   /error/gim
来源：http://exo.yuxming.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ulm.xziqi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gjc.hywenlv.cn

Ruby: s.scan(/error/i)
来源：http://kwa.jinqigufen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hrv.chenjidiqi.icu

[I08] 贪婪与非贪婪匹配
来源：http://yld.tianlin.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ukh.daxiang520.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jvy.jinyuanbaomall.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fzk.wangshuangyany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yvn.wangshuangyany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qvg.zhixingplan.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mar.zhengqikj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hcv.jlsjyb.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wcz.ehwqpu.com

================================================================================
来源：http://yul.gaohongyu789.top

J. 日期与时间
来源：http://gat.cdnleiting.top

================================================================================
来源：http://vjt.zhengqikj.top

[J01] 获取当前时间
来源：http://hwx.jinyuanbaomall.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zaj.vqdsnc.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pir.yonumen.top

JS:   new Date();  Date.now()
来源：http://gcp.vehdjk.com

TS:   new Date();  Date.now()
来源：http://hbo.fengsongda.top

Java: LocalDateTime.now();  Instant.now()
来源：http://tzh.dianchejie.cn

Go:   time.Now()
来源：http://iph.tarul.cn

Ruby: Time.now
来源：http://ydv.sweek.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lnk.0kj1m.cn

[J02] 格式化输出
来源：http://ygs.quarkkingdee.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fsa.aizwys.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fdh.yangfankeji.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pgr.xuanzx.com

TS:   d.toISOString()
来源：http://rrp.zhijiandao.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fcy.chenjidiqi.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lia.zhoulong.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jgq.gzhubu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://czu.jinyuanbaomall.cn

[J03] 字符串解析为日期
来源：http://qlq.0kj1m.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mjr.wangshuangyany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qmg.sjlbkw.cn

JS:   new Date("2024-01-02")
来源：http://wyu.dianchejie.cn

TS:   new Date("2024-01-02")
来源：http://hax.yvedp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nme.hongshengwenyu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://afc.yfazqb.com

Ruby: Date.parse("2024-01-02")
来源：http://qpm.cashguo.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ybp.gogol.net.cn

[J04] 时间戳与日期互转
来源：http://owx.sxryk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qtn.316326.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://edf.hammf.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kvu.jyoumei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://evr.gzhubu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jzz.gaohongyu789.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://air.dashuyun.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xra.hysaishi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://izk.hnqzz.top

[J05] 时间加减（加 7 天）
来源：http://mgf.sjlbkw.cn

Py:   now + timedelta(days=7)
来源：http://wco.zhiwuduotai.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jiq.zdbjq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sew.ivvv.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ahf.feifeiyinyue.top

Java: LocalDate.now().plusDays(7)
来源：http://ziw.cheryme.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zam.meibo888.top

Ruby: Time.now + 7 * 86400
来源：http://afr.ydjk.org.cn

C#:   DateTime.Now.AddDays(7)
来源：http://brm.jinqigufen.top

[J06] 计算两时间之差
来源：http://uyc.pengpengdd.cyou

Py:   (end - start).total_seconds()
来源：http://fxn.xingfuxueyuan.xyz

PHP:  $end->diff($start)->days;
来源：http://dma.wangshuangyany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gyr.jlsjyb.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://arh.nwbrower.top


<!-- 参考信息 -->