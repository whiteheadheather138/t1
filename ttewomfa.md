代发 wailian999

Java: interface Shape { double area(); }
来源：http://tdq.shanyushiyangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://pyu.shanyushiyangtech.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sjy.vqdsnc.cn

C#:   interface IShape { double Area(); }
来源：http://yaf.hnxiangtu.top

[G10] 访问控制
来源：http://jji.guannengcc.top

Py:   约定 _protected / __private（不强制）
来源：http://shh.snrcjt.cn

PHP:  public / protected / private
来源：http://ncx.nanxinkj.top

JS:   #private 字段；其余公开
来源：http://nht.zhoulong.xyz

TS:   public / protected / private
来源：http://bdm.snrcjt.cn

Java: public / protected / private / 默认包级
来源：http://seg.316326.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://vjn.yangfankeji.com

Ruby: public / protected / private
来源：http://nmk.yvedp.cn

C#:   public / protected / private / internal
来源：http://zuc.tarul.cn

[G11] getter / setter
来源：http://azp.zhoulong.xyz

Py:   @property 与 @x.setter
来源：http://skr.aibaodan.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hhv.jiagoushi.top

JS:   get name() { return this._name; }
来源：http://djn.vqdsnc.cn

TS:   get name(): string { return this._name; }
来源：http://uts.gzhubu.top

Java: public String getName() { return name; }
来源：http://nzo.mhx1999.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://kmv.ydjk.org.cn

Ruby: attr_accessor :name
来源：http://csh.jqgfzy.top

C#:   public string Name { get; set; }
来源：http://phs.wangshuangyany.cn

[G12] 对象转字符串
来源：http://wbr.jinqigufen.top

Py:   def __str__(self): return self.name
来源：http://hub.havefunace.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pqw.tarul.cn

JS:   toString() { return this.name; }
来源：http://pob.0kj1m.cn

TS:   toString(): string { return this.name; }
来源：http://dwr.hongshengwenyu.top

Java: @Override public String toString() { return name; }
来源：http://vuw.zdbjq.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vlv.sxryk.cn

Ruby: def to_s; @name; end
来源：http://wtx.hnqzz.top

C#:   public override string ToString() => Name;
来源：http://mqw.sysykeji.top

[G13] 判断对象类型
来源：http://npm.jqgufenzy.top

Py:   isinstance(u, User)
来源：http://hff.xziqi.cn

PHP:  $u instanceof User
来源：http://qbo.havefunace.top

JS:   u instanceof User
来源：http://iwm.snrcjt.cn

TS:   u instanceof User
来源：http://lwt.bjfxy.top

Java: u instanceof User
来源：http://alb.dashuyun.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vqe.tanke756.top

Ruby: u.is_a?(User)
来源：http://zrx.yuxming.cn

C#:   u is User
来源：http://wfl.ppjwa.cn

[G14] 数据类 / record
来源：http://nje.pengpengdd.cyou

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fwk.jianghu66.top

PHP:  // 用 readonly 属性模拟
来源：http://uyv.quarkkingdee.top

JS:   // 无内置：普通类或对象字面量
来源：http://bpz.xingfuxueyuan.xyz

TS:   type User = { name: string; age: number };
来源：http://nld.jqgfzy.top

Java: record User(String name, int age) {}
来源：http://dxm.jqgufenzy.top

Go:   type User struct { Name string; Age int }
来源：http://oov.hnxiangtu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nxj.svipenyu.cn

C#:   record User(string Name, int Age);
来源：http://scl.vqdsnc.cn

[G15] 枚举
来源：http://fjy.ctjpmb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fvd.tian-w.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zau.havefunace.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://toi.jinqigufen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mzw.52xcode.cn

Java: enum Color { RED, GREEN }
来源：http://qlq.ivvv.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fqr.tanke756.top

Ruby: Color = %i[red green].freeze
来源：http://zdm.jlsjyb.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pug.haohaochexian.top

[G16] 对象转数组 / 字典
来源：http://oky.chenlongwang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://btr.vqdsnc.cn

PHP:  get_object_vars($obj);
来源：http://wyh.sjlbkw.cn

JS:   Object.entries(obj)
来源：http://oag.52xcode.cn

TS:   Object.entries(obj)
来源：http://pcn.yj20258888.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lbg.chenzaomai.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://trt.ivvv.top

Ruby: obj.instance_variables
来源：http://shd.zhoulong.xyz

C#:   // 用反射或 System.Text.Json
来源：http://dsb.wangdashe.top

================================================================================
来源：http://hkh.yj20258888.top

H. 异常与错误处理
来源：http://ldy.tianlin.xyz

================================================================================
来源：http://edd.ppjwa.cn

[H01] try / catch 基础
来源：http://qod.fzhhl.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://duy.hesvh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hxm.zdqjudy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mwl.xingfuxueyuan.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://eys.xingfuxueyuan.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ybc.gotoacloud.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wrq.tanke756.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jto.chenlongwang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lbt.svipenyu.cn

[H02] finally / ensure 收尾
来源：http://tcw.havefunace.top

Py:   try: f()⏎finally: cleanup()
来源：http://fqg.snrcjt.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fdq.jinqigfzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://gvh.iojbl.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wlt.iojbl.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jrd.jlsjyb.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wia.hammf.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dci.svipenyu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qho.jlsjyb.cn

[H03] 主动抛出异常
来源：http://vci.yongpay.top

Py:   raise ValueError("错误信息")
来源：http://hqq.sweek.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rlk.zhaomingkeji.xyz

JS:   throw new Error("错误信息");
来源：http://xtc.yueranfly.top

TS:   throw new Error("错误信息");
来源：http://uhp.xuetiantiany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://enh.zhaomingkeji.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ntg.shzxlz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://has.daria6918.cn

C#:   throw new ArgumentException("错误信息");
来源：http://duc.aizwys.cn

[H04] 自定义异常类型
来源：http://rue.0kj1m.cn

Py:   class MyError(Exception): pass
来源：http://cmn.daria6918.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dvo.shuidangran.top

JS:   class MyError extends Error {}
来源：http://uwd.zhiwuduotai.top

TS:   class MyError extends Error {}
来源：http://lwl.iojbl.cn

Java: class MyException extends RuntimeException {}
来源：http://ljb.sjlbkw.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wru.wangdashe.top

Ruby: class MyError < StandardError; end
来源：http://aow.jinqigufen.top

C#:   class MyException : Exception {}
来源：http://lny.yongpay.top

[H05] 捕获特定类型
来源：http://aec.shanyushiyangkeji.top

Py:   except ValueError as e:
来源：http://pgh.xinyue.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://irc.guannengcc.top

JS:   if (e instanceof TypeError) {}
来源：http://emu.zhaomingkeji.xyz

TS:   if (e instanceof TypeError) {}
来源：http://zmu.yonumen.top

Java: catch (IOException | SQLException e) {}
来源：http://yjj.fanxiaobao.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eib.jinqigufen.top

Ruby: rescue ArgumentError => e
来源：http://iui.jinyuanbaomall.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ues.wangdashe.top

[H06] 可选值 / 空值安全访问
来源：http://eho.shzxlz.cn

Py:   value = d.get("k") or default
来源：http://rag.fehbvm.com

PHP:  $v = $d["k"] ?? null;
来源：http://chs.xinyue.icu

JS:   obj?.a?.b;  d ?? default
来源：http://tlr.52xcode.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dga.shuidangran.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ret.svipenyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://imw.cheryme.top

Ruby: d&.dig(:a, :b)
来源：http://mpd.nwbrower.top

C#:   obj?.A?.B ?? default
来源：http://igx.shanyushiyangtech.top

[H07] 断言
来源：http://zkg.iojbl.cn

Py:   assert x > 0, "必须为正"
来源：http://eta.pycfn.com

PHP:  assert($x > 0);
来源：http://ydn.0kj1m.cn

JS:   console.assert(x > 0);
来源：http://ntb.yj202588.top

TS:   console.assert(x > 0);
来源：http://hdv.zhijiandao.cn

Java: assert x > 0 : "必须为正";
来源：http://vnr.sxryk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ygy.hnqzz.top

Ruby: raise "必须为正" unless x > 0
来源：http://myz.havefunace.top

C#:   Debug.Assert(x > 0);
来源：http://xid.fktsv.cn

[H08] 获取错误信息与堆栈
来源：http://gai.jinqigfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://pqd.fengsongda.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rgj.yvedp.cn

JS:   e.message;  e.stack
来源：http://yhm.cqqwz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qhg.zhaomingkeji.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://hmv.daria6918.cn

Go:   err.Error()
来源：http://drj.nwbrower.top

Ruby: e.message;  e.backtrace
来源：http://ozo.zhijiandao.cn

C#:   e.Message;  e.StackTrace
来源：http://gko.jinyuanbaomall.cn

[H09] 带错误码的异常
来源：http://ztx.zhaomingkeji.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nue.316326.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://wdo.bjfxy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ixf.aizwys.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qyj.cqqwz.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://orz.zdbjq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qdf.hongshengwenyu.top

Ruby: raise MyError.new("fail", 500)
来源：http://mla.hnxiangtu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://lzy.yfazqb.com

[H10] 资源自动释放
来源：http://dwn.vehdjk.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://kjf.jiagoushi.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hod.cashguo.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rgi.vqdsnc.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vpu.zdbjq.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://azn.birdmap.top

Go:   defer f.Close()
来源：http://rjo.bjfxy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vmt.gzhubu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ifq.snrcjt.cn

================================================================================
来源：http://olv.yuxming.cn

I. 正则表达式
来源：http://zxr.zhoulong.xyz

================================================================================
来源：http://lav.xuanzx.com

[I01] 判断是否匹配
来源：http://kjk.xziqi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vmx.vqdsnc.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gpj.jqgufenzy.top

JS:   /\d+/.test(s)
来源：http://epp.yonumen.top

TS:   /\d+/.test(s)
来源：http://zjb.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xif.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jce.sjlbkw.cn

Ruby: s.match?(/\d+/)
来源：http://iah.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://phy.yj202588.top

[I02] 提取所有匹配
来源：http://bta.snrcjt.cn

Py:   re.findall(r"\d+", s)
来源：http://cvd.quarkkingdee.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cpa.wangshuangyany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xqu.yuanzhike.top

TS:   s.match(/\d+/g)
来源：http://amm.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mkv.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xsq.yj202588.top

Ruby: s.scan(/\d+/)
来源：http://vwh.hywenlv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bwk.fktsv.cn

[I03] 提取捕获分组
来源：http://eun.yuanzhike.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qao.jinghuilouyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://drx.shzxlz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://saq.smart0.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tnw.mhx1999.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qkt.meibo888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://boo.hesvh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jji.tarul.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ggn.sxryk.cn

[I04] 正则替换
来源：http://nez.cashguo.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fnf.haohaochexian.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pgc.guowangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://iln.xinyue.icu

TS:   s.replace(/\d+/g, "#")
来源：http://mwd.cdnleiting.top

Java: s.replaceAll("\\d+", "#")
来源：http://gta.jinqigfzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://afq.hnxiangtu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ubm.nanxuanxn.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://osi.hywenlv.cn

[I05] 按正则拆分
来源：http://gpi.hcnkem.com

Py:   re.split(r"\s*,\s*", s)
来源：http://vmg.pycfn.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://znp.nanxuanxn.top

JS:   s.split(/\s*,\s*/)
来源：http://gal.hesvh.cn

TS:   s.split(/\s*,\s*/)
来源：http://kxr.vehdjk.com

Java: s.split("\\s*,\\s*")
来源：http://tuc.yongpay.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://foi.ybcxt.top

Ruby: s.split(/\s*,\s*/)
来源：http://xjp.hfpthk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kvv.feifeiyinyue.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gsf.zycfv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jtl.yj20258888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lku.yonumen.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qoc.yvedp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rca.cqqwz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lsk.hesvh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lbs.jiagoushi.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ktv.zhiwuduotai.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kem.hfpthk.cn

[I07] 忽略大小写与多行模式
来源：http://mnk.daxiang520.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://amb.ydzc1.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gdh.havefunace.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ybe.quarkkingdee.top

TS:   /error/gim
来源：http://wfj.uphjek.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jfg.0kj1m.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xxt.xingfuxueyuan.xyz

Ruby: s.scan(/error/i)
来源：http://feu.xziqi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hws.wangdashe.top

[I08] 贪婪与非贪婪匹配
来源：http://cvj.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jsd.c1oappe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dhf.jyoumei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dpl.jlsjyb.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hds.chenlongwang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://brd.jqgfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lqd.shanyushiyangkeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ddz.yj202588.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://syy.sjlbkw.cn

================================================================================
来源：http://khy.jinyuanbaomall.cn

J. 日期与时间
来源：http://nzu.pengpengdd.cyou

================================================================================
来源：http://tfu.bjfxy.top

[J01] 获取当前时间
来源：http://nes.0kj1m.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ttt.gogol.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eay.smart0.xyz

JS:   new Date();  Date.now()
来源：http://zlt.hysaishi.cn

TS:   new Date();  Date.now()
来源：http://zxk.wangdashe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yov.jinqigufen.top

Go:   time.Now()
来源：http://mjl.yj202588.top

Ruby: Time.now
来源：http://dsu.fengsongda.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://eqy.gogol.net.cn

[J02] 格式化输出
来源：http://xbw.ppjwa.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dfi.jinqigfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lsz.andypj.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rea.smart0.xyz

TS:   d.toISOString()
来源：http://jhk.bbcook.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xyc.redwolf501.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nms.zdqjudy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tcx.gaohongyu789.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wzt.hcnkem.com

[J03] 字符串解析为日期
来源：http://qqu.redwolf501.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cvj.daria6918.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tgl.pengpengdd.cyou

JS:   new Date("2024-01-02")
来源：http://doi.9152youxi.cn

TS:   new Date("2024-01-02")
来源：http://scf.tian-w.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zml.shuidangran.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lzv.ehwqpu.com

Ruby: Date.parse("2024-01-02")
来源：http://rqf.zycfv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tnb.birdmap.top

[J04] 时间戳与日期互转
来源：http://gzy.svipenyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mhh.wangdashe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iay.zdbjq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eyk.jianghu66.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ehc.shangyingyoupin.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rwi.jqgufenzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wqo.c1oappe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hxm.wangshuangyany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yjs.gotoacloud.top

[J05] 时间加减（加 7 天）
来源：http://xxn.smart0.xyz

Py:   now + timedelta(days=7)
来源：http://enb.hesvh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dsd.pycfn.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tzw.gogol.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oou.316326.xyz

Java: LocalDate.now().plusDays(7)
来源：http://noy.sufxvd.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cpe.cheryme.top

Ruby: Time.now + 7 * 86400
来源：http://jpq.zhiwuduotai.top

C#:   DateTime.Now.AddDays(7)
来源：http://wcq.yuxming.cn

[J06] 计算两时间之差
来源：http://khr.mhx1999.top

Py:   (end - start).total_seconds()
来源：http://azd.shzxlz.cn

PHP:  $end->diff($start)->days;
来源：http://iuz.zhongyouzk.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nsa.cdnleiting.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lmz.yuxming.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jyq.zdbjq.cn

Go:   end.Sub(start).Hours()
来源：http://tsr.aibaodan.cn

Ruby: end - start                 # 返回秒数
来源：http://mnq.nanxuanxn.top

C#:   (end - start).TotalSeconds
来源：http://kzo.zhiwuduotai.top

[J07] 比较两个日期
来源：http://nrq.hnxiangtu.top

Py:   d1 < d2;  d1 == d2
来源：http://gpw.cheryme.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rfs.xziqi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://itp.jinyuanbaomall.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yxq.ctjpmb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ttp.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://moy.haohaochexian.top

Ruby: d1 < d2;  d1 == d2
来源：http://fkk.hnxiangtu.top


<!-- 参考信息 -->