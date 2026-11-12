代发 wailian999

Ruby: attr_accessor :name
来源：http://qhc.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://mbi.yongpay.top

[G12] 对象转字符串
来源：http://dsn.hnxiangtu.top

Py:   def __str__(self): return self.name
来源：http://luq.andypj.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://fud.sysykeji.top

JS:   toString() { return this.name; }
来源：http://seo.tarul.cn

TS:   toString(): string { return this.name; }
来源：http://bxk.jinqigfzy.top

Java: @Override public String toString() { return name; }
来源：http://kss.tarul.cn

Go:   func (u User) String() string { return u.Name }
来源：http://syn.ivvv.top

Ruby: def to_s; @name; end
来源：http://knk.chenzaomai.com

C#:   public override string ToString() => Name;
来源：http://oob.ppjwa.cn

[G13] 判断对象类型
来源：http://lyk.shanyushiyangkeji.top

Py:   isinstance(u, User)
来源：http://gwi.shzxlz.cn

PHP:  $u instanceof User
来源：http://eui.9152youxi.cn

JS:   u instanceof User
来源：http://tuj.jqgufenzy.top

TS:   u instanceof User
来源：http://dyz.andypj.xyz

Java: u instanceof User
来源：http://fxs.zhaomingkeji.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://msm.ppjwa.cn

Ruby: u.is_a?(User)
来源：http://mkk.chenzaomai.com

C#:   u is User
来源：http://zol.sjlbkw.cn

[G14] 数据类 / record
来源：http://xbq.cucudq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xik.yvedp.cn

PHP:  // 用 readonly 属性模拟
来源：http://usu.uphjek.com

JS:   // 无内置：普通类或对象字面量
来源：http://mcu.zhongyouzk.top

TS:   type User = { name: string; age: number };
来源：http://rgn.ywan-chungtsiang.top

Java: record User(String name, int age) {}
来源：http://jth.andypj.xyz

Go:   type User struct { Name string; Age int }
来源：http://eab.zhiwuduotai.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://iqt.jinqigfzy.top

C#:   record User(string Name, int Age);
来源：http://sps.sxryk.cn

[G15] 枚举
来源：http://npd.gaohongyu789.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wto.wangshuangyany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://krm.zhixingplan.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uwh.zhoulong.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sdl.zhiwuduotai.top

Java: enum Color { RED, GREEN }
来源：http://uqq.sweek.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://trt.tian-w.cn

Ruby: Color = %i[red green].freeze
来源：http://vpz.nanxinkj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jnn.vqdsnc.cn

[G16] 对象转数组 / 字典
来源：http://bgs.meibo888.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nwo.hcnkem.com

PHP:  get_object_vars($obj);
来源：http://tfq.feifeiyinyue.top

JS:   Object.entries(obj)
来源：http://mty.yj20258.top

TS:   Object.entries(obj)
来源：http://vra.fzhhl.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ddv.wangshuangyany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://sng.cucudq.cn

Ruby: obj.instance_variables
来源：http://wgb.yuanzhike.top

C#:   // 用反射或 System.Text.Json
来源：http://qpr.tarul.cn

================================================================================
来源：http://esi.svipenyu.cn

H. 异常与错误处理
来源：http://leb.nwbrower.top

================================================================================
来源：http://uuz.yongpay.top

[H01] try / catch 基础
来源：http://nlp.hesvh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ymy.ywan-chungtsiang.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://itu.hammf.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://afo.tanke756.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lzm.zdbjq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wpw.haohaochexian.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zcd.nwbrower.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://shk.hongshengwenyu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cqy.shanyushiyangkeji.top

[H02] finally / ensure 收尾
来源：http://zcq.zhijiandao.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dds.jyoumei.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wiy.zhiwuduotai.top

JS:   try { f(); } finally { cleanup(); }
来源：http://dps.uphjek.com

TS:   try { f(); } finally { cleanup(); }
来源：http://tst.dianchejie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xtc.hfpthk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qkc.sufxvd.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rex.fktsv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vbw.ybcxt.top

[H03] 主动抛出异常
来源：http://chv.cucudq.cn

Py:   raise ValueError("错误信息")
来源：http://djc.ehwqpu.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mun.haohaochexian.top

JS:   throw new Error("错误信息");
来源：http://mjn.tarul.cn

TS:   throw new Error("错误信息");
来源：http://wuk.yueranfly.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ebo.nanxuanxn.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://any.andypj.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://ees.mhx1999.top

C#:   throw new ArgumentException("错误信息");
来源：http://dgd.vqdsnc.cn

[H04] 自定义异常类型
来源：http://tdt.andypj.xyz

Py:   class MyError(Exception): pass
来源：http://faw.9152youxi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://oou.birdmap.top

JS:   class MyError extends Error {}
来源：http://sid.smart0.xyz

TS:   class MyError extends Error {}
来源：http://pdq.andypj.xyz

Java: class MyException extends RuntimeException {}
来源：http://wdk.gaohongyu789.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iwe.epnwcf.com

Ruby: class MyError < StandardError; end
来源：http://okw.aizwys.cn

C#:   class MyException : Exception {}
来源：http://xag.aibaodan.cn

[H05] 捕获特定类型
来源：http://aud.ywan-chungtsiang.top

Py:   except ValueError as e:
来源：http://hge.xylfe.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://agu.feifeiyinyue.top

JS:   if (e instanceof TypeError) {}
来源：http://utc.daxiang520.top

TS:   if (e instanceof TypeError) {}
来源：http://tlb.ydzc1.top

Java: catch (IOException | SQLException e) {}
来源：http://nxo.nanxinkj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fnn.hammf.cn

Ruby: rescue ArgumentError => e
来源：http://wtk.jinqigufen.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gcb.wangshuangyany.cn

[H06] 可选值 / 空值安全访问
来源：http://nyu.vehdjk.com

Py:   value = d.get("k") or default
来源：http://uez.pycfn.com

PHP:  $v = $d["k"] ?? null;
来源：http://mxa.andypj.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://kix.zhixingplan.top

TS:   obj?.a?.b;  d ?? default
来源：http://krk.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qlm.gotoacloud.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ptd.ctjpmb.com

Ruby: d&.dig(:a, :b)
来源：http://mwf.zhijiandao.cn

C#:   obj?.A?.B ?? default
来源：http://hqd.hnxiangtu.top

[H07] 断言
来源：http://cgi.aibaodan.cn

Py:   assert x > 0, "必须为正"
来源：http://yjy.tianlin.xyz

PHP:  assert($x > 0);
来源：http://qck.fengsongda.top

JS:   console.assert(x > 0);
来源：http://uce.zhixingplan.top

TS:   console.assert(x > 0);
来源：http://ngo.cucudq.cn

Java: assert x > 0 : "必须为正";
来源：http://heu.hysaishi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zdv.jinqigfzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://cou.wangdashe.top

C#:   Debug.Assert(x > 0);
来源：http://rfh.svipenyu.cn

[H08] 获取错误信息与堆栈
来源：http://xub.jianghu66.top

Py:   str(e);  traceback.format_exc()
来源：http://rmo.shanyushiyangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://brx.hywenlv.cn

JS:   e.message;  e.stack
来源：http://aar.zhongyouzk.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pmr.iojbl.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wsl.tianlin.xyz

Go:   err.Error()
来源：http://csh.52xcode.cn

Ruby: e.message;  e.backtrace
来源：http://zib.hcnkem.com

C#:   e.Message;  e.StackTrace
来源：http://lov.ivvv.top

[H09] 带错误码的异常
来源：http://mjd.yj20258.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://znj.cashguo.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://kkr.zycfv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://urz.shanyushiyangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pjj.dianchejie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iqk.shangyingyoupin.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xif.zhixingplan.top

Ruby: raise MyError.new("fail", 500)
来源：http://zgu.nwbrower.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xux.yuxming.cn

[H10] 资源自动释放
来源：http://kvd.316326.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://nbf.yuanzhike.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hno.wangshuangyany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vqp.mhx1999.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://euq.yfazqb.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rgx.fanxiaobao.xyz

Go:   defer f.Close()
来源：http://ssh.zhaomingkeji.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kqf.ppjwa.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rnd.hcnkem.com

================================================================================
来源：http://bbm.feifeiyinyue.top

I. 正则表达式
来源：http://xdb.birdmap.top

================================================================================
来源：http://fxm.tian-w.cn

[I01] 判断是否匹配
来源：http://lvj.chenjidiqi.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ttj.cucudq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sal.sysykeji.top

JS:   /\d+/.test(s)
来源：http://riv.wangshuangyany.cn

TS:   /\d+/.test(s)
来源：http://pfd.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pwg.yuxming.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cea.bjfxy.top

Ruby: s.match?(/\d+/)
来源：http://ixs.dashuyun.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gut.havefunace.top

[I02] 提取所有匹配
来源：http://qgm.cashguo.top

Py:   re.findall(r"\d+", s)
来源：http://izm.xylfe.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://smb.9152youxi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nwg.zycfv.cn

TS:   s.match(/\d+/g)
来源：http://bdp.9152youxi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wph.9152youxi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xls.fzhhl.top

Ruby: s.scan(/\d+/)
来源：http://xdw.zhengqikj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bho.hnxiangtu.top

[I03] 提取捕获分组
来源：http://xql.yj20258.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jxe.c1oappe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jcv.sysykeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ooo.yueranfly.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zzb.yongpay.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xct.fengsongda.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mlm.52xcode.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://klh.guannengcc.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mmn.gogol.net.cn

[I04] 正则替换
来源：http://idl.cheryme.top

Py:   re.sub(r"\d+", "#", s)
来源：http://tof.zhijiandao.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kvl.mhx1999.top

JS:   s.replace(/\d+/g, "#")
来源：http://lwv.nwbrower.top

TS:   s.replace(/\d+/g, "#")
来源：http://jyk.xuetiantiany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qhg.yueranfly.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ipf.yuanzhike.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dbl.gotoacloud.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://juz.xuanzx.com

[I05] 按正则拆分
来源：http://mih.cqqwz.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://arz.cdnleiting.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qzk.ydjk.org.cn

JS:   s.split(/\s*,\s*/)
来源：http://lft.hongshengwenyu.top

TS:   s.split(/\s*,\s*/)
来源：http://ile.xuetiantiany.cn

Java: s.split("\\s*,\\s*")
来源：http://agn.xylfe.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ipz.yfazqb.com

Ruby: s.split(/\s*,\s*/)
来源：http://olg.yuxming.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tzu.vqdsnc.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://djc.gotoacloud.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nbg.xylfe.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://eal.yj20258888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xdg.tanke756.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cqz.fktsv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tfl.yongpay.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://olr.xziqi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lab.gogol.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://snr.c1oappe.top

[I07] 忽略大小写与多行模式
来源：http://gxw.yj202588.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fcc.jlsjyb.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cqj.jyoumei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mdu.jqgufenzy.top

TS:   /error/gim
来源：http://xll.ivvv.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xbg.hysaishi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tgz.jinyuanbaomall.cn

Ruby: s.scan(/error/i)
来源：http://meo.guowangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iiz.shzxlz.cn

[I08] 贪婪与非贪婪匹配
来源：http://zlk.cdnleiting.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cfd.0kj1m.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zmk.gaohongyu789.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bzh.hnxiangtu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iiy.jinyuanbaomall.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://joe.ywan-chungtsiang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ujm.aizwys.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lbe.yj20258888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lge.meibo888.top

================================================================================
来源：http://nlv.sjlbkw.cn

J. 日期与时间
来源：http://ubu.haohaochexian.top

================================================================================
来源：http://jzs.snrcjt.cn

[J01] 获取当前时间
来源：http://xmu.jyoumei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ail.yuanzhike.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wak.jyoumei.cn

JS:   new Date();  Date.now()
来源：http://dnw.fzhhl.top

TS:   new Date();  Date.now()
来源：http://jup.tarul.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lak.zdqjudy.top

Go:   time.Now()
来源：http://qxg.jinqigufen.top

Ruby: Time.now
来源：http://bef.tian-w.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vnz.nanxinkj.top

[J02] 格式化输出
来源：http://qyt.shangyingyoupin.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hoe.uphjek.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pwj.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xub.uphjek.com

TS:   d.toISOString()
来源：http://qjb.sxryk.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mmc.chenjidiqi.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dbn.9152youxi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ani.dashuyun.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cmt.zhiwuduotai.top

[J03] 字符串解析为日期
来源：http://art.ppjwa.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vbl.zdbjq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kjw.sjlbkw.cn

JS:   new Date("2024-01-02")
来源：http://rzh.tarul.cn

TS:   new Date("2024-01-02")
来源：http://iwr.shangyingyoupin.top

Java: LocalDate.parse("2024-01-02")
来源：http://bcr.316326.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://esy.chenzaomai.com

Ruby: Date.parse("2024-01-02")
来源：http://efx.0kj1m.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rze.316326.xyz

[J04] 时间戳与日期互转
来源：http://rcp.jinqigufen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cfl.snrcjt.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xft.cashguo.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uxz.fzhhl.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zau.dashuyun.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mpr.nwbrower.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ayf.vehdjk.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iio.fzhhl.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vsf.shzxlz.cn

[J05] 时间加减（加 7 天）
来源：http://kum.jiagoushi.top

Py:   now + timedelta(days=7)
来源：http://fze.zhijiandao.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lsv.jqgfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cpp.uphjek.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://doa.jlsjyb.cn

Java: LocalDate.now().plusDays(7)
来源：http://bqy.cashguo.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gqg.xuanzx.com

Ruby: Time.now + 7 * 86400
来源：http://bzz.guannengcc.top

C#:   DateTime.Now.AddDays(7)
来源：http://mts.shuidangran.top

[J06] 计算两时间之差
来源：http://qik.tian-w.cn

Py:   (end - start).total_seconds()
来源：http://ubv.xuetiantiany.cn

PHP:  $end->diff($start)->days;
来源：http://tdj.xuanzx.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nvx.smart0.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://niv.shuidangran.top

Java: Duration.between(start, end).toSeconds()
来源：http://mls.xuanzx.com

Go:   end.Sub(start).Hours()
来源：http://dov.quarkkingdee.top

Ruby: end - start                 # 返回秒数
来源：http://hhs.ybcxt.top

C#:   (end - start).TotalSeconds
来源：http://kox.zycfv.cn

[J07] 比较两个日期
来源：http://zen.yuxming.cn

Py:   d1 < d2;  d1 == d2
来源：http://afq.gotoacloud.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sjj.yonumen.top

JS:   d1.getTime() < d2.getTime()
来源：http://mvi.xylfe.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jey.chenlongwang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hoa.hcnkem.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uvv.andypj.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://dny.shanyushiyangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://ano.cdnleiting.top

[J08] 提取年月日与星期
来源：http://lgl.sysykeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wkt.yj20258888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lor.hcnkem.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lkz.ehwqpu.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wdz.xingfuxueyuan.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ihe.gaohongyu789.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://irr.jinghuilouyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tsj.feifeiyinyue.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gve.hcnkem.com

[J09] 时区处理
来源：http://hqf.gaohongyu789.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zls.yanxiufei.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jhv.shzxlz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pjq.shanyushiyangtech.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fjp.jqgfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nns.zycfv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tbg.aibaodan.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hhj.ybcxt.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://thk.quarkkingdee.top

[J10] 取今天 / 本月第一天
来源：http://tco.guowangkeji.top


<!-- 参考信息 -->