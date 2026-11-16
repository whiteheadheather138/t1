代发 wailian999

JS:   get name() { return this._name; }
来源：http://cgj.vqdsnc.cn

TS:   get name(): string { return this._name; }
来源：http://zyz.zhongyouzk.top

Java: public String getName() { return name; }
来源：http://cot.snrcjt.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rda.feifeiyinyue.top

Ruby: attr_accessor :name
来源：http://pcw.shuidangran.top

C#:   public string Name { get; set; }
来源：http://gvg.xinyue.icu

[G12] 对象转字符串
来源：http://jrf.fanxiaobao.xyz

Py:   def __str__(self): return self.name
来源：http://ocq.bbcook.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gme.52xcode.cn

JS:   toString() { return this.name; }
来源：http://usb.yueranfly.top

TS:   toString(): string { return this.name; }
来源：http://dwu.aizwys.cn

Java: @Override public String toString() { return name; }
来源：http://bre.shanyushiyangtech.top

Go:   func (u User) String() string { return u.Name }
来源：http://ydw.yj202588.top

Ruby: def to_s; @name; end
来源：http://uch.xuanzx.com

C#:   public override string ToString() => Name;
来源：http://dpn.fanxiaobao.xyz

[G13] 判断对象类型
来源：http://jql.jianghu66.top

Py:   isinstance(u, User)
来源：http://myh.tanke756.top

PHP:  $u instanceof User
来源：http://krp.hongshengwenyu.top

JS:   u instanceof User
来源：http://ixs.yanxiufei.cn

TS:   u instanceof User
来源：http://ppb.bjfxy.top

Java: u instanceof User
来源：http://oei.shanyushiyangtech.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://egm.52xcode.cn

Ruby: u.is_a?(User)
来源：http://sku.0kj1m.cn

C#:   u is User
来源：http://vml.xziqi.cn

[G14] 数据类 / record
来源：http://oxg.ivvv.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wzx.pengpengdd.cyou

PHP:  // 用 readonly 属性模拟
来源：http://fjb.jlsjyb.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wzj.ehwqpu.com

TS:   type User = { name: string; age: number };
来源：http://xxa.hnxiangtu.top

Java: record User(String name, int age) {}
来源：http://ory.zhixingplan.top

Go:   type User struct { Name string; Age int }
来源：http://duc.gaohongyu789.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pyl.aibaodan.cn

C#:   record User(string Name, int Age);
来源：http://zyz.sjlbkw.cn

[G15] 枚举
来源：http://pkl.epnwcf.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wks.zhixingplan.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hwx.zhoulong.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fhw.guannengcc.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vrt.xylfe.cn

Java: enum Color { RED, GREEN }
来源：http://unv.tianlin.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ifa.zycfv.cn

Ruby: Color = %i[red green].freeze
来源：http://duv.havefunace.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ara.birdmap.top

[G16] 对象转数组 / 字典
来源：http://yso.gzhubu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://obd.c1oappe.top

PHP:  get_object_vars($obj);
来源：http://mjw.yanxiufei.cn

JS:   Object.entries(obj)
来源：http://gwz.dashuyun.cn

TS:   Object.entries(obj)
来源：http://mqg.pengpengdd.cyou

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hgc.hywenlv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mhl.shuidangran.top

Ruby: obj.instance_variables
来源：http://tgc.fzhhl.top

C#:   // 用反射或 System.Text.Json
来源：http://thx.xylfe.cn

================================================================================
来源：http://qwg.jinqigufen.top

H. 异常与错误处理
来源：http://utx.yanxiufei.cn

================================================================================
来源：http://xbn.shangyingyoupin.top

[H01] try / catch 基础
来源：http://kyf.snrcjt.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fpu.sweek.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dra.guowangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jqm.dashuyun.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://epp.yuxming.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tsr.hysaishi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://msa.yangfankeji.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ztl.yanxiufei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nfe.ydjk.org.cn

[H02] finally / ensure 收尾
来源：http://wug.nanxuanxn.top

Py:   try: f()⏎finally: cleanup()
来源：http://ldo.jinghuilouyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mgp.shanyushiyangtech.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zhy.316326.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://lgp.shzxlz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://imd.vqdsnc.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://snv.guannengcc.top

Ruby: begin; f; ensure; cleanup; end
来源：http://tor.uphjek.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://dzy.zhoulong.xyz

[H03] 主动抛出异常
来源：http://rgb.c1oappe.top

Py:   raise ValueError("错误信息")
来源：http://ugs.meibo888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dgh.hesvh.cn

JS:   throw new Error("错误信息");
来源：http://mha.zhijiandao.cn

TS:   throw new Error("错误信息");
来源：http://tmu.meibo888.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ogh.hnxiangtu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mwj.shanyushiyangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jnb.aibaodan.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jsq.snrcjt.cn

[H04] 自定义异常类型
来源：http://aqn.hysaishi.cn

Py:   class MyError(Exception): pass
来源：http://zti.shanyushiyangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://swd.xinyue.icu

JS:   class MyError extends Error {}
来源：http://iqm.hongshengwenyu.top

TS:   class MyError extends Error {}
来源：http://ium.zdbjq.cn

Java: class MyException extends RuntimeException {}
来源：http://tle.dashuyun.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://spl.zhongyouzk.top

Ruby: class MyError < StandardError; end
来源：http://gle.chenlongwang.top

C#:   class MyException : Exception {}
来源：http://sgn.hcnkem.com

[H05] 捕获特定类型
来源：http://zal.cqqwz.cn

Py:   except ValueError as e:
来源：http://kwu.aizwys.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://idm.zycfv.cn

JS:   if (e instanceof TypeError) {}
来源：http://xyq.birdmap.top

TS:   if (e instanceof TypeError) {}
来源：http://ajx.snrcjt.cn

Java: catch (IOException | SQLException e) {}
来源：http://cqx.chenzaomai.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kjw.xuanzx.com

Ruby: rescue ArgumentError => e
来源：http://ctl.zhongyouzk.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pac.hnqzz.top

[H06] 可选值 / 空值安全访问
来源：http://xuz.mhx1999.top

Py:   value = d.get("k") or default
来源：http://oll.fehbvm.com

PHP:  $v = $d["k"] ?? null;
来源：http://uad.zdqjudy.top

JS:   obj?.a?.b;  d ?? default
来源：http://wrz.wangdashe.top

TS:   obj?.a?.b;  d ?? default
来源：http://pow.jqgfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vdi.zycfv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yei.jinqigufen.top

Ruby: d&.dig(:a, :b)
来源：http://ycy.aibaodan.cn

C#:   obj?.A?.B ?? default
来源：http://zuu.ivvv.top

[H07] 断言
来源：http://jab.dashuyun.cn

Py:   assert x > 0, "必须为正"
来源：http://lqt.nanxuanxn.top

PHP:  assert($x > 0);
来源：http://gho.cdnleiting.top

JS:   console.assert(x > 0);
来源：http://ikx.jyoumei.cn

TS:   console.assert(x > 0);
来源：http://kcj.bjfxy.top

Java: assert x > 0 : "必须为正";
来源：http://kug.cdnleiting.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fww.pengpengdd.cyou

Ruby: raise "必须为正" unless x > 0
来源：http://lbe.cdnleiting.top

C#:   Debug.Assert(x > 0);
来源：http://gtv.yangfankeji.com

[H08] 获取错误信息与堆栈
来源：http://epl.316326.xyz

Py:   str(e);  traceback.format_exc()
来源：http://ein.jiagoushi.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://imx.zdbjq.cn

JS:   e.message;  e.stack
来源：http://mzu.yj20258888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://aog.sjlbkw.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uib.cucudq.cn

Go:   err.Error()
来源：http://myx.zhaomingkeji.xyz

Ruby: e.message;  e.backtrace
来源：http://ffo.ehwqpu.com

C#:   e.Message;  e.StackTrace
来源：http://ltc.andypj.xyz

[H09] 带错误码的异常
来源：http://olc.hysaishi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gpj.pengpengdd.cyou

PHP:  throw new RuntimeException("fail", 500);
来源：http://zzv.shanyushiyangtech.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bbt.hongshengwenyu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ogo.yanxiufei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fbu.hysaishi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://apl.xylfe.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yus.quarkkingdee.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fym.zdbjq.cn

[H10] 资源自动释放
来源：http://eqj.ybcxt.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ipx.hfpthk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jkt.shanyushiyangtech.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lzf.cashguo.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vum.xziqi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jgl.bjfxy.top

Go:   defer f.Close()
来源：http://eqd.havefunace.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cgk.jinyuanbaomall.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nze.jqgufenzy.top

================================================================================
来源：http://veu.tianlin.xyz

I. 正则表达式
来源：http://oib.guowangkeji.top

================================================================================
来源：http://bty.daxiang520.top

[I01] 判断是否匹配
来源：http://kgh.0kj1m.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xhu.aizwys.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kdn.yuanzhike.top

JS:   /\d+/.test(s)
来源：http://hlg.yuxming.cn

TS:   /\d+/.test(s)
来源：http://ilh.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nbv.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vqy.daria6918.cn

Ruby: s.match?(/\d+/)
来源：http://ibt.shzxlz.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://woa.birdmap.top

[I02] 提取所有匹配
来源：http://iki.sjlbkw.cn

Py:   re.findall(r"\d+", s)
来源：http://xgm.nanxinkj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mqp.xziqi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kxt.xuetiantiany.cn

TS:   s.match(/\d+/g)
来源：http://zbc.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ygn.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sxb.chenjidiqi.icu

Ruby: s.scan(/\d+/)
来源：http://iln.haohaochexian.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uib.zdqjudy.top

[I03] 提取捕获分组
来源：http://syc.chenzaomai.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lzt.yj20258.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://brc.mhx1999.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bki.yj20258888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ato.c1oappe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mpg.jqgfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nix.xziqi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://arf.dashuyun.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://soy.zhiwuduotai.top

[I04] 正则替换
来源：http://ppx.shanyushiyangtech.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gyr.fktsv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kph.0kj1m.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xkd.zhiwuduotai.top

TS:   s.replace(/\d+/g, "#")
来源：http://ysi.fehbvm.com

Java: s.replaceAll("\\d+", "#")
来源：http://puf.sjlbkw.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pbw.chenlongwang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qaw.ydzc1.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wkq.pycfn.com

[I05] 按正则拆分
来源：http://ufv.dashuyun.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mti.hnqzz.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uno.tianlin.xyz

JS:   s.split(/\s*,\s*/)
来源：http://hkf.hongshengwenyu.top

TS:   s.split(/\s*,\s*/)
来源：http://nbw.sysykeji.top

Java: s.split("\\s*,\\s*")
来源：http://lxg.iojbl.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iin.cheryme.top

Ruby: s.split(/\s*,\s*/)
来源：http://ici.zhengqikj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eix.zhijiandao.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eee.sjlbkw.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ftl.hywenlv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mhq.zhiwuduotai.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bnz.gzhubu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rou.zhoulong.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vjv.zhiwuduotai.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jbi.hesvh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://aar.zdbjq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ieh.yanxiufei.cn

[I07] 忽略大小写与多行模式
来源：http://lnz.yvedp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bku.hnxiangtu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mlj.jinqigufen.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lne.yueranfly.top

TS:   /error/gim
来源：http://yvr.zdqjudy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mrf.hongshengwenyu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://iae.gzhubu.top

Ruby: s.scan(/error/i)
来源：http://bbu.52xcode.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wry.fengsongda.top

[I08] 贪婪与非贪婪匹配
来源：http://oqt.gogol.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gbz.hywenlv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xdq.yueranfly.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bwy.xuetiantiany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iik.jianghu66.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mct.cqqwz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://orx.9152youxi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uty.yanxiufei.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ggb.sysykeji.top

================================================================================
来源：http://sjl.iojbl.cn

J. 日期与时间
来源：http://pxo.bbcook.cn

================================================================================
来源：http://wvk.cqqwz.cn

[J01] 获取当前时间
来源：http://qag.yj20258.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://rjs.yj20258.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lyg.yonumen.top

JS:   new Date();  Date.now()
来源：http://ipl.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://syg.zdqjudy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://kml.zhiwuduotai.top

Go:   time.Now()
来源：http://kte.cucudq.cn

Ruby: Time.now
来源：http://fpp.jinghuilouyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mvc.hywenlv.cn

[J02] 格式化输出
来源：http://rqj.hnqzz.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tib.jqgufenzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eie.jianghu66.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ypt.uphjek.com

TS:   d.toISOString()
来源：http://huu.zhoulong.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://csm.hesvh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nji.ivvv.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mpg.vqdsnc.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jxj.tarul.cn

[J03] 字符串解析为日期
来源：http://uyj.guannengcc.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bdz.feifeiyinyue.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kmn.cqqwz.cn

JS:   new Date("2024-01-02")
来源：http://rjn.ppjwa.cn

TS:   new Date("2024-01-02")
来源：http://qbo.yanxiufei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pon.jinqigfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://frs.zdbjq.cn

Ruby: Date.parse("2024-01-02")
来源：http://jef.tianlin.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://scr.cucudq.cn

[J04] 时间戳与日期互转
来源：http://tbd.yanxiufei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kxh.sweek.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rik.kuanghao11.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xyf.xuanzx.com

TS:   Math.floor(Date.now() / 1000)
来源：http://ene.yonumen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bwj.vehdjk.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cqi.andypj.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kvl.wangdashe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qfc.gaohongyu789.top

[J05] 时间加减（加 7 天）
来源：http://vdr.ybcxt.top

Py:   now + timedelta(days=7)
来源：http://duz.shangyingyoupin.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://evd.yonumen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cfn.zdqjudy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xui.yuanzhike.top

Java: LocalDate.now().plusDays(7)
来源：http://qpi.gzhubu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wbz.yonumen.top

Ruby: Time.now + 7 * 86400
来源：http://nbj.9152youxi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vwi.chenlongwang.top

[J06] 计算两时间之差
来源：http://yqc.zhijiandao.cn

Py:   (end - start).total_seconds()
来源：http://ooo.zhijiandao.cn

PHP:  $end->diff($start)->days;
来源：http://elm.yanxiufei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wld.jinghuilouyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eln.tian-w.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hps.ehwqpu.com

Go:   end.Sub(start).Hours()
来源：http://ovz.sxryk.cn

Ruby: end - start                 # 返回秒数
来源：http://fgv.gaohongyu789.top

C#:   (end - start).TotalSeconds
来源：http://xnr.chenjidiqi.icu

[J07] 比较两个日期
来源：http://ofe.vehdjk.com

Py:   d1 < d2;  d1 == d2
来源：http://htc.vqdsnc.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wwd.snrcjt.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hjv.yangfankeji.com

TS:   d1.getTime() < d2.getTime()
来源：http://gsq.xylfe.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cxn.zhaomingkeji.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wbr.daria6918.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gza.ydzc1.top

C#:   d1 < d2;  d1 == d2
来源：http://bpg.ydjk.org.cn

[J08] 提取年月日与星期
来源：http://kmy.jlsjyb.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ggy.zhoulong.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bai.bjfxy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lkg.tarul.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ckf.yuxming.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cnu.yuxming.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fpu.ppjwa.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qlo.birdmap.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kjk.shangyingyoupin.top

[J09] 时区处理
来源：http://cwp.hesvh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://usd.zhaomingkeji.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hnu.chenlongwang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dbd.ivvv.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ktp.epnwcf.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ggk.vehdjk.com


<!-- 参考信息 -->