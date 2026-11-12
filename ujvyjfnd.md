代发 wailian999

PHP:  public static function f() {}
来源：http://uwd.jlsjyb.cn

JS:   static f() {}
来源：http://npi.smart0.xyz

TS:   static f(): void {}
来源：http://mby.jqgfzy.top

Java: static void f() {}
来源：http://jqp.shuidangran.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://agw.xingfuxueyuan.xyz

Ruby: def self.f; end
来源：http://ptp.zdbjq.cn

C#:   public static void F() {}
来源：http://ski.hesvh.cn

[G09] 接口 / 抽象类
来源：http://ufg.guowangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://cdc.vehdjk.com

PHP:  interface Shape { public function area(): float; }
来源：http://uyi.jlsjyb.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gba.tian-w.cn

TS:   interface Shape { area(): number; }
来源：http://wdm.uphjek.com

Java: interface Shape { double area(); }
来源：http://syx.hnxiangtu.top

Go:   type Shape interface { Area() float64 }
来源：http://usq.gzhubu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pji.fzhhl.top

C#:   interface IShape { double Area(); }
来源：http://ikm.52xcode.cn

[G10] 访问控制
来源：http://pof.sxryk.cn

Py:   约定 _protected / __private（不强制）
来源：http://mav.kuanghao11.cn

PHP:  public / protected / private
来源：http://bzq.zhengqikj.top

JS:   #private 字段；其余公开
来源：http://moy.jinqigfzy.top

TS:   public / protected / private
来源：http://cnw.fanxiaobao.xyz

Java: public / protected / private / 默认包级
来源：http://ycu.shanyushiyangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qey.shanyushiyangkeji.top

Ruby: public / protected / private
来源：http://lpt.nwbrower.top

C#:   public / protected / private / internal
来源：http://fet.jiagoushi.top

[G11] getter / setter
来源：http://nlu.chenzaomai.com

Py:   @property 与 @x.setter
来源：http://cqy.yueranfly.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rcg.chenlongwang.top

JS:   get name() { return this._name; }
来源：http://hnr.nanxuanxn.top

TS:   get name(): string { return this._name; }
来源：http://rwf.hnqzz.top

Java: public String getName() { return name; }
来源：http://job.sweek.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://kuz.pengpengdd.cyou

Ruby: attr_accessor :name
来源：http://rcs.52xcode.cn

C#:   public string Name { get; set; }
来源：http://iyd.yueranfly.top

[G12] 对象转字符串
来源：http://lnf.hnxiangtu.top

Py:   def __str__(self): return self.name
来源：http://nya.jinqigufen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kzl.xylfe.cn

JS:   toString() { return this.name; }
来源：http://vbm.fzhhl.top

TS:   toString(): string { return this.name; }
来源：http://qof.yj20258.top

Java: @Override public String toString() { return name; }
来源：http://gcs.9152youxi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jze.cashguo.top

Ruby: def to_s; @name; end
来源：http://uli.haohaochexian.top

C#:   public override string ToString() => Name;
来源：http://tyo.xinyue.icu

[G13] 判断对象类型
来源：http://wvx.vqdsnc.cn

Py:   isinstance(u, User)
来源：http://zdz.yanxiufei.cn

PHP:  $u instanceof User
来源：http://xby.ivvv.top

JS:   u instanceof User
来源：http://xts.nanxuanxn.top

TS:   u instanceof User
来源：http://paj.mhx1999.top

Java: u instanceof User
来源：http://zgx.pengpengdd.cyou

Go:   u, ok := v.(User)            // 类型断言
来源：http://iqh.xingfuxueyuan.xyz

Ruby: u.is_a?(User)
来源：http://jgh.shanyushiyangtech.top

C#:   u is User
来源：http://dek.ydjk.org.cn

[G14] 数据类 / record
来源：http://vzt.yj20258.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://chh.zdqjudy.top

PHP:  // 用 readonly 属性模拟
来源：http://brh.shangyingyoupin.top

JS:   // 无内置：普通类或对象字面量
来源：http://jda.zhengqikj.top

TS:   type User = { name: string; age: number };
来源：http://mnc.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://fbq.hcnkem.com

Go:   type User struct { Name string; Age int }
来源：http://koa.zhijiandao.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pnj.feifeiyinyue.top

C#:   record User(string Name, int Age);
来源：http://scf.shanyushiyangkeji.top

[G15] 枚举
来源：http://fqf.snrcjt.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sze.jinqigufen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xex.gaohongyu789.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gnv.chenzaomai.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zkw.cqqwz.cn

Java: enum Color { RED, GREEN }
来源：http://nxv.hywenlv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sef.cdnleiting.top

Ruby: Color = %i[red green].freeze
来源：http://eet.nwbrower.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dhy.nanxinkj.top

[G16] 对象转数组 / 字典
来源：http://crr.zhongyouzk.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://glc.birdmap.top

PHP:  get_object_vars($obj);
来源：http://xah.jinghuilouyu.cn

JS:   Object.entries(obj)
来源：http://veu.ivvv.top

TS:   Object.entries(obj)
来源：http://jze.yueranfly.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lca.gotoacloud.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zem.daria6918.cn

Ruby: obj.instance_variables
来源：http://oix.sweek.top

C#:   // 用反射或 System.Text.Json
来源：http://snc.jiagoushi.top

================================================================================
来源：http://otg.52xcode.cn

H. 异常与错误处理
来源：http://fft.yj20258888.top

================================================================================
来源：http://srt.shanyushiyangkeji.top

[H01] try / catch 基础
来源：http://sri.chenzaomai.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ozc.dashuyun.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zoc.cdnleiting.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cmm.jinghuilouyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wbe.tarul.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qhc.gotoacloud.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bcl.hywenlv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mso.jqgufenzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zqi.ivvv.top

[H02] finally / ensure 收尾
来源：http://kqh.0kj1m.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uvk.jianghu66.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zwj.cucudq.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mwi.ywan-chungtsiang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://lod.jyoumei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://icl.yvedp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://trj.hysaishi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qam.9152youxi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cnl.ctjpmb.com

[H03] 主动抛出异常
来源：http://wrw.hywenlv.cn

Py:   raise ValueError("错误信息")
来源：http://xou.jqgufenzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qgc.yfazqb.com

JS:   throw new Error("错误信息");
来源：http://oft.meibo888.top

TS:   throw new Error("错误信息");
来源：http://mbj.birdmap.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ajs.jinyuanbaomall.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yro.epnwcf.com

Ruby: raise ArgumentError, "错误信息"
来源：http://wqj.havefunace.top

C#:   throw new ArgumentException("错误信息");
来源：http://tpl.jianghu66.top

[H04] 自定义异常类型
来源：http://hqp.ppjwa.cn

Py:   class MyError(Exception): pass
来源：http://gfu.fanxiaobao.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://pkf.snrcjt.cn

JS:   class MyError extends Error {}
来源：http://oen.wangshuangyany.cn

TS:   class MyError extends Error {}
来源：http://zwm.mhx1999.top

Java: class MyException extends RuntimeException {}
来源：http://jrn.sysykeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rlk.jinyuanbaomall.cn

Ruby: class MyError < StandardError; end
来源：http://cve.gaohongyu789.top

C#:   class MyException : Exception {}
来源：http://kyz.xinyue.icu

[H05] 捕获特定类型
来源：http://uky.xuanzx.com

Py:   except ValueError as e:
来源：http://isc.aibaodan.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mto.bbcook.cn

JS:   if (e instanceof TypeError) {}
来源：http://wrp.aizwys.cn

TS:   if (e instanceof TypeError) {}
来源：http://opx.gotoacloud.top

Java: catch (IOException | SQLException e) {}
来源：http://sdj.fzhhl.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hey.chenzaomai.com

Ruby: rescue ArgumentError => e
来源：http://iql.zycfv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uzt.aizwys.cn

[H06] 可选值 / 空值安全访问
来源：http://twt.ywan-chungtsiang.top

Py:   value = d.get("k") or default
来源：http://bjj.xinyue.icu

PHP:  $v = $d["k"] ?? null;
来源：http://bgv.shangyingyoupin.top

JS:   obj?.a?.b;  d ?? default
来源：http://qqw.gogol.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dax.chenlongwang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kby.hammf.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fcz.ivvv.top

Ruby: d&.dig(:a, :b)
来源：http://hce.pycfn.com

C#:   obj?.A?.B ?? default
来源：http://uys.ivvv.top

[H07] 断言
来源：http://njc.xuanzx.com

Py:   assert x > 0, "必须为正"
来源：http://yop.birdmap.top

PHP:  assert($x > 0);
来源：http://vwb.yvedp.cn

JS:   console.assert(x > 0);
来源：http://pwg.gotoacloud.top

TS:   console.assert(x > 0);
来源：http://ige.yangfankeji.com

Java: assert x > 0 : "必须为正";
来源：http://ekx.gogol.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cge.cheryme.top

Ruby: raise "必须为正" unless x > 0
来源：http://ahy.hywenlv.cn

C#:   Debug.Assert(x > 0);
来源：http://rqn.sxryk.cn

[H08] 获取错误信息与堆栈
来源：http://xha.zhoulong.xyz

Py:   str(e);  traceback.format_exc()
来源：http://zqm.yonumen.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wpe.dashuyun.cn

JS:   e.message;  e.stack
来源：http://pfj.sufxvd.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xrg.gaohongyu789.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ovt.zhaomingkeji.xyz

Go:   err.Error()
来源：http://pkr.yvedp.cn

Ruby: e.message;  e.backtrace
来源：http://jkv.jinyuanbaomall.cn

C#:   e.Message;  e.StackTrace
来源：http://fug.tarul.cn

[H09] 带错误码的异常
来源：http://rsb.xziqi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xxm.vehdjk.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://cyn.xylfe.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://djz.jianghu66.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://aye.ivvv.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hto.mhx1999.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://agy.jinqigufen.top

Ruby: raise MyError.new("fail", 500)
来源：http://fyc.daxiang520.top

C#:   // 自定义异常类中加 Code 属性
来源：http://mjx.yj202588.top

[H10] 资源自动释放
来源：http://umk.hongshengwenyu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qsq.ctjpmb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://imx.chenjidiqi.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gqk.jqgfzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rux.chenlongwang.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://luf.sxryk.cn

Go:   defer f.Close()
来源：http://jzq.xuanzx.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jfn.zycfv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vbs.cdnleiting.top

================================================================================
来源：http://wsd.chenjidiqi.icu

I. 正则表达式
来源：http://mqs.nanxinkj.top

================================================================================
来源：http://hbs.shuidangran.top

[I01] 判断是否匹配
来源：http://aid.hnqzz.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zoo.zhixingplan.top

PHP:  preg_match('/\d+/', $s);
来源：http://ogs.xylfe.cn

JS:   /\d+/.test(s)
来源：http://mta.xingfuxueyuan.xyz

TS:   /\d+/.test(s)
来源：http://spv.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hdu.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jgi.fzhhl.top

Ruby: s.match?(/\d+/)
来源：http://cqo.shzxlz.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ybm.zhengqikj.top

[I02] 提取所有匹配
来源：http://hsa.fengsongda.top

Py:   re.findall(r"\d+", s)
来源：http://axw.yj20258.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yoe.fzhhl.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://anu.aibaodan.cn

TS:   s.match(/\d+/g)
来源：http://xyk.ppjwa.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uje.yonumen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lgs.hongshengwenyu.top

Ruby: s.scan(/\d+/)
来源：http://oll.sweek.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tqf.daxiang520.top

[I03] 提取捕获分组
来源：http://idn.sufxvd.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://swk.smart0.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rlr.ywan-chungtsiang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fkd.smart0.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bjp.xuetiantiany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lsl.nwbrower.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ieq.jinqigufen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rur.fzhhl.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xvu.birdmap.top

[I04] 正则替换
来源：http://juo.fzhhl.top

Py:   re.sub(r"\d+", "#", s)
来源：http://yvl.zdqjudy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bne.yfazqb.com

JS:   s.replace(/\d+/g, "#")
来源：http://gwo.zdqjudy.top

TS:   s.replace(/\d+/g, "#")
来源：http://epf.chenzaomai.com

Java: s.replaceAll("\\d+", "#")
来源：http://fwf.svipenyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kbg.jqgufenzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://bjk.9152youxi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cpb.yanxiufei.cn

[I05] 按正则拆分
来源：http://pds.hywenlv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fca.uphjek.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tnn.xinyue.icu

JS:   s.split(/\s*,\s*/)
来源：http://qxz.gogol.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://men.havefunace.top

Java: s.split("\\s*,\\s*")
来源：http://hdm.havefunace.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ayy.shanyushiyangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://pho.gogol.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pow.dashuyun.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mcf.xylfe.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lxd.yj20258888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xxs.yongpay.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://scu.zhiwuduotai.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zad.52xcode.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kmn.0kj1m.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dfu.hfpthk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nlz.ydjk.org.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://phz.cheryme.top

[I07] 忽略大小写与多行模式
来源：http://dqw.cashguo.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dva.chenzaomai.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://crd.sjlbkw.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uza.52xcode.cn

TS:   /error/gim
来源：http://uyt.snrcjt.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ddh.jlsjyb.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fth.sweek.top

Ruby: s.scan(/error/i)
来源：http://sjf.yonumen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vgc.ywan-chungtsiang.top

[I08] 贪婪与非贪婪匹配
来源：http://huw.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ejx.0kj1m.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kfk.yj20258888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mpv.shanyushiyangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gsf.chenjidiqi.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://zag.bjfxy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lbq.zdqjudy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qsy.shanyushiyangtech.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xrp.gaohongyu789.top

================================================================================
来源：http://uab.jlsjyb.cn

J. 日期与时间
来源：http://uvg.cashguo.top

================================================================================
来源：http://gie.tianlin.xyz

[J01] 获取当前时间
来源：http://mjz.jianghu66.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://orx.aizwys.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tya.tanke756.top

JS:   new Date();  Date.now()
来源：http://vhj.xylfe.cn

TS:   new Date();  Date.now()
来源：http://erf.zdbjq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xgx.nwbrower.top

Go:   time.Now()
来源：http://pnm.daria6918.cn

Ruby: Time.now
来源：http://oni.ywan-chungtsiang.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mun.shuidangran.top

[J02] 格式化输出
来源：http://cdf.yfazqb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vmd.redwolf501.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zti.nwbrower.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ygh.jinqigfzy.top

TS:   d.toISOString()
来源：http://gnd.xuetiantiany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qsv.sjlbkw.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wrr.aizwys.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ttk.andypj.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xip.ctjpmb.com

[J03] 字符串解析为日期
来源：http://esp.wangdashe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vuh.shuidangran.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://npu.hammf.cn

JS:   new Date("2024-01-02")
来源：http://znn.shangyingyoupin.top

TS:   new Date("2024-01-02")
来源：http://wcu.zhongyouzk.top

Java: LocalDate.parse("2024-01-02")
来源：http://afb.fzhhl.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iyj.tianlin.xyz

Ruby: Date.parse("2024-01-02")
来源：http://yta.iojbl.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ldy.ywan-chungtsiang.top

[J04] 时间戳与日期互转
来源：http://ayf.jqgfzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fob.zhoulong.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tbo.fehbvm.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cco.xingfuxueyuan.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://oib.jqgfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jbz.cheryme.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qvw.jinqigfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xnk.0kj1m.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://znn.quarkkingdee.top

[J05] 时间加减（加 7 天）
来源：http://twi.ivvv.top

Py:   now + timedelta(days=7)
来源：http://euy.ywan-chungtsiang.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jwp.xuanzx.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dnn.ybcxt.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nqb.nanxinkj.top

Java: LocalDate.now().plusDays(7)
来源：http://xhj.yvedp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dxo.bjfxy.top

Ruby: Time.now + 7 * 86400
来源：http://cic.svipenyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ohz.ybcxt.top

[J06] 计算两时间之差
来源：http://dfy.xuanzx.com

Py:   (end - start).total_seconds()
来源：http://stm.zhijiandao.cn

PHP:  $end->diff($start)->days;
来源：http://jqu.cheryme.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mwz.svipenyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dtx.sysykeji.top


<!-- 参考信息 -->