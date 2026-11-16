代发 wailian999

Ruby: attr_accessor :name
来源：http://fis.fehbvm.com

C#:   public string Name { get; set; }
来源：http://qlc.zhiwuduotai.top

[G12] 对象转字符串
来源：http://xuc.jinqigfzy.top

Py:   def __str__(self): return self.name
来源：http://bgt.tian-w.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://asj.jianghu66.top

JS:   toString() { return this.name; }
来源：http://jav.chenjidiqi.icu

TS:   toString(): string { return this.name; }
来源：http://jrw.guannengcc.top

Java: @Override public String toString() { return name; }
来源：http://juy.tarul.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zei.xinyue.icu

Ruby: def to_s; @name; end
来源：http://iwg.ctjpmb.com

C#:   public override string ToString() => Name;
来源：http://urt.nwbrower.top

[G13] 判断对象类型
来源：http://zqm.nwbrower.top

Py:   isinstance(u, User)
来源：http://fxj.wangdashe.top

PHP:  $u instanceof User
来源：http://mwy.ivvv.top

JS:   u instanceof User
来源：http://upm.yonumen.top

TS:   u instanceof User
来源：http://tzw.yonumen.top

Java: u instanceof User
来源：http://kuy.hcnkem.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://tfp.zycfv.cn

Ruby: u.is_a?(User)
来源：http://bac.316326.xyz

C#:   u is User
来源：http://dav.fzhhl.top

[G14] 数据类 / record
来源：http://yus.ywan-chungtsiang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://eun.quarkkingdee.top

PHP:  // 用 readonly 属性模拟
来源：http://ctp.jinqigfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://jku.yj20258.top

TS:   type User = { name: string; age: number };
来源：http://ixk.jinyuanbaomall.cn

Java: record User(String name, int age) {}
来源：http://vij.daxiang520.top

Go:   type User struct { Name string; Age int }
来源：http://wqy.xziqi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://erm.yfazqb.com

C#:   record User(string Name, int Age);
来源：http://rzs.jinqigufen.top

[G15] 枚举
来源：http://kmx.zdbjq.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nwj.c1oappe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://klt.hongshengwenyu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rsn.zhoulong.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pby.wangshuangyany.cn

Java: enum Color { RED, GREEN }
来源：http://btv.shanyushiyangkeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lzf.gaohongyu789.top

Ruby: Color = %i[red green].freeze
来源：http://quz.jinqigufen.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qlf.snrcjt.cn

[G16] 对象转数组 / 字典
来源：http://whk.shzxlz.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uhx.zhiwuduotai.top

PHP:  get_object_vars($obj);
来源：http://zmu.sysykeji.top

JS:   Object.entries(obj)
来源：http://fnn.9152youxi.cn

TS:   Object.entries(obj)
来源：http://wwr.316326.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xqv.hfpthk.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dvt.yangfankeji.com

Ruby: obj.instance_variables
来源：http://fke.gotoacloud.top

C#:   // 用反射或 System.Text.Json
来源：http://upz.yuanzhike.top

================================================================================
来源：http://crw.yj202588.top

H. 异常与错误处理
来源：http://xnx.epnwcf.com

================================================================================
来源：http://rgc.0kj1m.cn

[H01] try / catch 基础
来源：http://zid.hesvh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gtf.xziqi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rfl.cashguo.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://esz.epnwcf.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ijv.pycfn.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tjt.nanxinkj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gsd.iojbl.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yak.wangshuangyany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mjv.shanyushiyangkeji.top

[H02] finally / ensure 收尾
来源：http://dhh.yvedp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dgl.uphjek.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://iko.zycfv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mgl.quarkkingdee.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ouw.fktsv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wtn.zhijiandao.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zce.wangdashe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mwe.smart0.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://bnr.shanyushiyangtech.top

[H03] 主动抛出异常
来源：http://ssv.pycfn.com

Py:   raise ValueError("错误信息")
来源：http://oxc.xuetiantiany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://aei.52xcode.cn

JS:   throw new Error("错误信息");
来源：http://ajd.meibo888.top

TS:   throw new Error("错误信息");
来源：http://boj.ppjwa.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hcu.vqdsnc.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wfm.fanxiaobao.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://wgy.52xcode.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lll.hysaishi.cn

[H04] 自定义异常类型
来源：http://vad.sufxvd.cn

Py:   class MyError(Exception): pass
来源：http://znp.sweek.top

PHP:  class MyError extends RuntimeException {}
来源：http://cwy.9152youxi.cn

JS:   class MyError extends Error {}
来源：http://sdl.ydjk.org.cn

TS:   class MyError extends Error {}
来源：http://jpr.havefunace.top

Java: class MyException extends RuntimeException {}
来源：http://ktk.chenzaomai.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dvl.sysykeji.top

Ruby: class MyError < StandardError; end
来源：http://fvf.yongpay.top

C#:   class MyException : Exception {}
来源：http://nqr.havefunace.top

[H05] 捕获特定类型
来源：http://soc.c1oappe.top

Py:   except ValueError as e:
来源：http://hou.uphjek.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zti.yj202588.top

JS:   if (e instanceof TypeError) {}
来源：http://wpo.chenjidiqi.icu

TS:   if (e instanceof TypeError) {}
来源：http://xun.zhoulong.xyz

Java: catch (IOException | SQLException e) {}
来源：http://tgo.ehwqpu.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jvr.yueranfly.top

Ruby: rescue ArgumentError => e
来源：http://wsb.jlsjyb.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ctx.zhiwuduotai.top

[H06] 可选值 / 空值安全访问
来源：http://cuz.316326.xyz

Py:   value = d.get("k") or default
来源：http://qbg.yj20258888.top

PHP:  $v = $d["k"] ?? null;
来源：http://uzs.pycfn.com

JS:   obj?.a?.b;  d ?? default
来源：http://epj.hcnkem.com

TS:   obj?.a?.b;  d ?? default
来源：http://rak.xuetiantiany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yjf.svipenyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bca.sjlbkw.cn

Ruby: d&.dig(:a, :b)
来源：http://unl.nanxinkj.top

C#:   obj?.A?.B ?? default
来源：http://awb.jqgufenzy.top

[H07] 断言
来源：http://ovv.pycfn.com

Py:   assert x > 0, "必须为正"
来源：http://ypf.xuanzx.com

PHP:  assert($x > 0);
来源：http://ppq.zhijiandao.cn

JS:   console.assert(x > 0);
来源：http://rsi.sxryk.cn

TS:   console.assert(x > 0);
来源：http://qve.zhixingplan.top

Java: assert x > 0 : "必须为正";
来源：http://yyy.xziqi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ccg.hesvh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ghv.zycfv.cn

C#:   Debug.Assert(x > 0);
来源：http://tvl.quarkkingdee.top

[H08] 获取错误信息与堆栈
来源：http://vah.snrcjt.cn

Py:   str(e);  traceback.format_exc()
来源：http://bhm.gaohongyu789.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cwv.hfpthk.cn

JS:   e.message;  e.stack
来源：http://kiq.zdqjudy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lon.nanxinkj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pvw.pengpengdd.cyou

Go:   err.Error()
来源：http://zdk.daria6918.cn

Ruby: e.message;  e.backtrace
来源：http://jlr.pycfn.com

C#:   e.Message;  e.StackTrace
来源：http://gzn.jinghuilouyu.cn

[H09] 带错误码的异常
来源：http://rig.nanxuanxn.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ciq.ybcxt.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jvi.vehdjk.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lyp.hesvh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lgd.fktsv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ivc.hcnkem.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mrz.feifeiyinyue.top

Ruby: raise MyError.new("fail", 500)
来源：http://evl.cqqwz.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bnr.mhx1999.top

[H10] 资源自动释放
来源：http://lyb.jqgufenzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ffh.zhongyouzk.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tdv.yangfankeji.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://okt.shuidangran.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mhq.yj20258888.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lfg.iojbl.cn

Go:   defer f.Close()
来源：http://qcl.gaohongyu789.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mmq.vehdjk.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lno.yfazqb.com

================================================================================
来源：http://qjy.hesvh.cn

I. 正则表达式
来源：http://kus.52xcode.cn

================================================================================
来源：http://ppa.zhiwuduotai.top

[I01] 判断是否匹配
来源：http://rhz.fengsongda.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ajg.jinghuilouyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nna.jinqigfzy.top

JS:   /\d+/.test(s)
来源：http://hzs.zdqjudy.top

TS:   /\d+/.test(s)
来源：http://bla.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nte.c1oappe.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://srs.zhoulong.xyz

Ruby: s.match?(/\d+/)
来源：http://ixr.jinqigufen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://oil.dianchejie.cn

[I02] 提取所有匹配
来源：http://rtm.xinyue.icu

Py:   re.findall(r"\d+", s)
来源：http://lcb.ehwqpu.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wzs.chenlongwang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://niz.yvedp.cn

TS:   s.match(/\d+/g)
来源：http://knd.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cci.hfpthk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gyi.zhiwuduotai.top

Ruby: s.scan(/\d+/)
来源：http://rzh.nanxuanxn.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jey.havefunace.top

[I03] 提取捕获分组
来源：http://sdk.zycfv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ynk.jinyuanbaomall.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://woc.sufxvd.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zmm.tanke756.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uwa.fengsongda.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tlt.52xcode.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gnx.ehwqpu.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nlf.guowangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kgd.gzhubu.top

[I04] 正则替换
来源：http://xuy.vqdsnc.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wdc.gzhubu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://asa.vqdsnc.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dmi.xinyue.icu

TS:   s.replace(/\d+/g, "#")
来源：http://whx.kuanghao11.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lpd.jqgufenzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wda.sxryk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bep.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ihq.hywenlv.cn

[I05] 按正则拆分
来源：http://wja.aizwys.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zcc.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://asz.redwolf501.top

JS:   s.split(/\s*,\s*/)
来源：http://lzz.zhengqikj.top

TS:   s.split(/\s*,\s*/)
来源：http://ipx.dashuyun.cn

Java: s.split("\\s*,\\s*")
来源：http://afg.fktsv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rws.feifeiyinyue.top

Ruby: s.split(/\s*,\s*/)
来源：http://dou.svipenyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tfu.zhiwuduotai.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nmi.zhoulong.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mnz.zhongyouzk.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mqm.zdqjudy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://isv.xylfe.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nyb.tanke756.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://att.cheryme.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://far.ywan-chungtsiang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qed.ybcxt.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bbd.hnxiangtu.top

[I07] 忽略大小写与多行模式
来源：http://wcd.svipenyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rtk.bjfxy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qcf.xuanzx.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://isk.yonumen.top

TS:   /error/gim
来源：http://meu.wangshuangyany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dyz.kuanghao11.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cvm.yueranfly.top

Ruby: s.scan(/error/i)
来源：http://uxf.snrcjt.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qtq.hfpthk.cn

[I08] 贪婪与非贪婪匹配
来源：http://trv.52xcode.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qjn.yonumen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ewz.xuanzx.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zia.sufxvd.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xqm.sufxvd.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zco.ivvv.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sqe.xuanzx.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ieg.uphjek.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gpb.zycfv.cn

================================================================================
来源：http://xxo.hnxiangtu.top

J. 日期与时间
来源：http://qhk.birdmap.top

================================================================================
来源：http://jdt.0kj1m.cn

[J01] 获取当前时间
来源：http://ikm.xuetiantiany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gus.hnqzz.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tle.snrcjt.cn

JS:   new Date();  Date.now()
来源：http://bgz.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://jfc.shanyushiyangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://beh.sufxvd.cn

Go:   time.Now()
来源：http://jvb.pycfn.com

Ruby: Time.now
来源：http://axw.52xcode.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kop.tanke756.top

[J02] 格式化输出
来源：http://ugf.nanxinkj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qxs.aizwys.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jnj.feifeiyinyue.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://azk.xziqi.cn

TS:   d.toISOString()
来源：http://hln.shangyingyoupin.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ofe.gotoacloud.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ccb.yongpay.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uty.daria6918.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hyo.meibo888.top

[J03] 字符串解析为日期
来源：http://kab.jiagoushi.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mcs.dashuyun.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pxm.fehbvm.com

JS:   new Date("2024-01-02")
来源：http://blv.jqgufenzy.top

TS:   new Date("2024-01-02")
来源：http://wqh.fzhhl.top

Java: LocalDate.parse("2024-01-02")
来源：http://puw.shuidangran.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nib.cheryme.top

Ruby: Date.parse("2024-01-02")
来源：http://zxj.ehwqpu.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hvf.9152youxi.cn

[J04] 时间戳与日期互转
来源：http://scy.birdmap.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mqk.ppjwa.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fwf.daria6918.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cif.shuidangran.top

TS:   Math.floor(Date.now() / 1000)
来源：http://hrc.yfazqb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ulq.smart0.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kmf.guannengcc.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://spn.pengpengdd.cyou

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kso.jqgufenzy.top

[J05] 时间加减（加 7 天）
来源：http://nxb.gogol.net.cn

Py:   now + timedelta(days=7)
来源：http://wor.zhaomingkeji.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://rhe.cucudq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rpc.hesvh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lfc.bjfxy.top

Java: LocalDate.now().plusDays(7)
来源：http://orm.ydzc1.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pxw.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://dfe.fehbvm.com

C#:   DateTime.Now.AddDays(7)
来源：http://vvi.uphjek.com

[J06] 计算两时间之差
来源：http://ppg.iojbl.cn

Py:   (end - start).total_seconds()
来源：http://sby.pengpengdd.cyou

PHP:  $end->diff($start)->days;
来源：http://mfh.yuanzhike.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://idh.jinqigfzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eqr.gotoacloud.top

Java: Duration.between(start, end).toSeconds()
来源：http://lfl.ctjpmb.com

Go:   end.Sub(start).Hours()
来源：http://ijf.jqgfzy.top

Ruby: end - start                 # 返回秒数
来源：http://ujm.yfazqb.com

C#:   (end - start).TotalSeconds
来源：http://kpp.havefunace.top

[J07] 比较两个日期
来源：http://rtg.shzxlz.cn

Py:   d1 < d2;  d1 == d2
来源：http://jtu.nanxinkj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ind.daxiang520.top

JS:   d1.getTime() < d2.getTime()
来源：http://fmk.hongshengwenyu.top

TS:   d1.getTime() < d2.getTime()
来源：http://uwz.hongshengwenyu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://iad.hnxiangtu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://keu.redwolf501.top

Ruby: d1 < d2;  d1 == d2
来源：http://jcf.chenlongwang.top

C#:   d1 < d2;  d1 == d2
来源：http://bwu.jiagoushi.top

[J08] 提取年月日与星期
来源：http://oja.sjlbkw.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rqa.zhiwuduotai.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://iop.ydjk.org.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rqr.xuetiantiany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://maq.bbcook.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aan.xuanzx.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pwe.quarkkingdee.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dmq.nanxinkj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dlw.cheryme.top

[J09] 时区处理
来源：http://ixu.shuidangran.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://suw.cdnleiting.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ycj.yonumen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vld.jiagoushi.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xqh.fehbvm.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://psg.jianghu66.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vis.iojbl.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ezx.yj20258888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ytq.xuanzx.com

[J10] 取今天 / 本月第一天
来源：http://ufr.hysaishi.cn


<!-- 参考信息 -->