代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://tel.zhongyouzk.top

Java: record User(String name, int age) {}
来源：http://sod.dashuyun.cn

Go:   type User struct { Name string; Age int }
来源：http://nvo.fktsv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://frw.vqdsnc.cn

C#:   record User(string Name, int Age);
来源：http://nhf.epnwcf.com

[G15] 枚举
来源：http://urr.pengpengdd.cyou

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fpf.snrcjt.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dkj.gaohongyu789.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ipd.fengsongda.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://srp.hnxiangtu.top

Java: enum Color { RED, GREEN }
来源：http://zll.andypj.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://utx.zdqjudy.top

Ruby: Color = %i[red green].freeze
来源：http://qua.meibo888.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zhl.yongpay.top

[G16] 对象转数组 / 字典
来源：http://dfp.gogol.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tkz.sufxvd.cn

PHP:  get_object_vars($obj);
来源：http://amy.jinqigufen.top

JS:   Object.entries(obj)
来源：http://kgv.yongpay.top

TS:   Object.entries(obj)
来源：http://kjg.jinyuanbaomall.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xrk.yongpay.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://djv.ppjwa.cn

Ruby: obj.instance_variables
来源：http://zsm.feifeiyinyue.top

C#:   // 用反射或 System.Text.Json
来源：http://nfg.jyoumei.cn

================================================================================
来源：http://csf.xingfuxueyuan.xyz

H. 异常与错误处理
来源：http://vpn.shzxlz.cn

================================================================================
来源：http://vtf.svipenyu.cn

[H01] try / catch 基础
来源：http://ela.hfpthk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nza.shanyushiyangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ulp.jinghuilouyu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cme.fzhhl.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mxv.jiagoushi.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xaj.daxiang520.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tio.fehbvm.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dxy.hywenlv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rdp.jianghu66.top

[H02] finally / ensure 收尾
来源：http://gnm.ehwqpu.com

Py:   try: f()⏎finally: cleanup()
来源：http://fov.zycfv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mcp.daxiang520.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qrx.feifeiyinyue.top

TS:   try { f(); } finally { cleanup(); }
来源：http://geu.daria6918.cn

Java: try { f(); } finally { cleanup(); }
来源：http://nnd.chenzaomai.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://srx.meibo888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://baj.pengpengdd.cyou

C#:   try { F(); } finally { Cleanup(); }
来源：http://wnf.yangfankeji.com

[H03] 主动抛出异常
来源：http://grf.zhijiandao.cn

Py:   raise ValueError("错误信息")
来源：http://pgc.iojbl.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xwm.feifeiyinyue.top

JS:   throw new Error("错误信息");
来源：http://izk.jinqigfzy.top

TS:   throw new Error("错误信息");
来源：http://cqe.epnwcf.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://qzc.fehbvm.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yrx.ctjpmb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://xmt.jiagoushi.top

C#:   throw new ArgumentException("错误信息");
来源：http://mkn.pengpengdd.cyou

[H04] 自定义异常类型
来源：http://knf.bjfxy.top

Py:   class MyError(Exception): pass
来源：http://fya.hcnkem.com

PHP:  class MyError extends RuntimeException {}
来源：http://xke.316326.xyz

JS:   class MyError extends Error {}
来源：http://glb.jinyuanbaomall.cn

TS:   class MyError extends Error {}
来源：http://ixe.uphjek.com

Java: class MyException extends RuntimeException {}
来源：http://cuc.vqdsnc.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ouv.bbcook.cn

Ruby: class MyError < StandardError; end
来源：http://eon.birdmap.top

C#:   class MyException : Exception {}
来源：http://ywx.zhengqikj.top

[H05] 捕获特定类型
来源：http://ywf.9152youxi.cn

Py:   except ValueError as e:
来源：http://xqd.ydjk.org.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jjg.shanyushiyangtech.top

JS:   if (e instanceof TypeError) {}
来源：http://hgz.hammf.cn

TS:   if (e instanceof TypeError) {}
来源：http://lsu.tianlin.xyz

Java: catch (IOException | SQLException e) {}
来源：http://pjv.yueranfly.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eel.52xcode.cn

Ruby: rescue ArgumentError => e
来源：http://wpp.sjlbkw.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jqd.jinqigufen.top

[H06] 可选值 / 空值安全访问
来源：http://hmy.feifeiyinyue.top

Py:   value = d.get("k") or default
来源：http://hgt.sxryk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sgj.52xcode.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pwe.zhixingplan.top

TS:   obj?.a?.b;  d ?? default
来源：http://yzi.shanyushiyangtech.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xks.yj20258888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vlr.0kj1m.cn

Ruby: d&.dig(:a, :b)
来源：http://iai.xinyue.icu

C#:   obj?.A?.B ?? default
来源：http://nja.chenlongwang.top

[H07] 断言
来源：http://tfn.uphjek.com

Py:   assert x > 0, "必须为正"
来源：http://fhs.cashguo.top

PHP:  assert($x > 0);
来源：http://ybp.zhoulong.xyz

JS:   console.assert(x > 0);
来源：http://tfj.yueranfly.top

TS:   console.assert(x > 0);
来源：http://wtb.yvedp.cn

Java: assert x > 0 : "必须为正";
来源：http://fml.hcnkem.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://brj.yj20258.top

Ruby: raise "必须为正" unless x > 0
来源：http://qnb.nwbrower.top

C#:   Debug.Assert(x > 0);
来源：http://clq.yj20258888.top

[H08] 获取错误信息与堆栈
来源：http://jvs.316326.xyz

Py:   str(e);  traceback.format_exc()
来源：http://jix.svipenyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gqp.snrcjt.cn

JS:   e.message;  e.stack
来源：http://duy.ydzc1.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://dln.vehdjk.com

Java: e.getMessage();  e.printStackTrace()
来源：http://tne.fzhhl.top

Go:   err.Error()
来源：http://fmj.jinyuanbaomall.cn

Ruby: e.message;  e.backtrace
来源：http://obg.sjlbkw.cn

C#:   e.Message;  e.StackTrace
来源：http://zqm.hysaishi.cn

[H09] 带错误码的异常
来源：http://iar.iojbl.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wnp.dashuyun.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dvy.zhongyouzk.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gxn.fktsv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eig.fktsv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tbm.nanxuanxn.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ojg.zhaomingkeji.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://vnl.shuidangran.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gmv.dianchejie.cn

[H10] 资源自动释放
来源：http://fya.sufxvd.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://loc.nanxinkj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gzu.havefunace.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yen.hnqzz.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jyn.xingfuxueyuan.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dbc.tian-w.cn

Go:   defer f.Close()
来源：http://quf.gotoacloud.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hms.jyoumei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uly.kuanghao11.cn

================================================================================
来源：http://stb.cheryme.top

I. 正则表达式
来源：http://jkg.sufxvd.cn

================================================================================
来源：http://ned.hnqzz.top

[I01] 判断是否匹配
来源：http://hln.smart0.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lov.gotoacloud.top

PHP:  preg_match('/\d+/', $s);
来源：http://phz.zdbjq.cn

JS:   /\d+/.test(s)
来源：http://erc.hesvh.cn

TS:   /\d+/.test(s)
来源：http://vpi.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fyv.cheryme.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nsm.hcnkem.com

Ruby: s.match?(/\d+/)
来源：http://qfw.ppjwa.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xpe.shanyushiyangkeji.top

[I02] 提取所有匹配
来源：http://vrj.zhijiandao.cn

Py:   re.findall(r"\d+", s)
来源：http://mls.nwbrower.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vxp.shanyushiyangtech.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://adn.pycfn.com

TS:   s.match(/\d+/g)
来源：http://fzj.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ntu.ivvv.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bad.zhiwuduotai.top

Ruby: s.scan(/\d+/)
来源：http://tss.jlsjyb.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vdp.fengsongda.top

[I03] 提取捕获分组
来源：http://qfv.nanxuanxn.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vek.bjfxy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lvk.daxiang520.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uul.tian-w.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kfz.tarul.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xmu.zhijiandao.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ubw.yuxming.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cnb.hnxiangtu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nef.ivvv.top

[I04] 正则替换
来源：http://jet.yvedp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://luu.xziqi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cks.havefunace.top

JS:   s.replace(/\d+/g, "#")
来源：http://cuo.c1oappe.top

TS:   s.replace(/\d+/g, "#")
来源：http://fvy.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://sga.yj20258.top

Go:   re.ReplaceAllString(s, "#")
来源：http://klc.xinyue.icu

Ruby: s.gsub(/\d+/, "#")
来源：http://iny.sysykeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://abi.xylfe.cn

[I05] 按正则拆分
来源：http://faz.smart0.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://jlz.jinyuanbaomall.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ahh.jinqigufen.top

JS:   s.split(/\s*,\s*/)
来源：http://lvz.yonumen.top

TS:   s.split(/\s*,\s*/)
来源：http://ryi.tianlin.xyz

Java: s.split("\\s*,\\s*")
来源：http://ciy.chenzaomai.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ftj.hysaishi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nze.ivvv.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ahm.feifeiyinyue.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kwc.snrcjt.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://erk.iojbl.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://est.xylfe.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zcl.hnqzz.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kwl.pycfn.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tbt.hnqzz.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eky.wangshuangyany.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xyv.ydzc1.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vsy.hammf.cn

[I07] 忽略大小写与多行模式
来源：http://qyh.chenzaomai.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yuw.zdqjudy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tqf.yuanzhike.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jue.hnxiangtu.top

TS:   /error/gim
来源：http://twr.jqgfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jaj.hnqzz.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sia.wangdashe.top

Ruby: s.scan(/error/i)
来源：http://ssi.ctjpmb.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://feu.tarul.cn

[I08] 贪婪与非贪婪匹配
来源：http://wib.guowangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yhj.jinyuanbaomall.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vez.vqdsnc.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zvs.0kj1m.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://unr.fanxiaobao.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://bab.xziqi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pmk.pengpengdd.cyou

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mws.ydjk.org.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ugd.quarkkingdee.top

================================================================================
来源：http://xff.sjlbkw.cn

J. 日期与时间
来源：http://fts.yj202588.top

================================================================================
来源：http://rda.gzhubu.top

[J01] 获取当前时间
来源：http://edw.xinyue.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://lpt.cheryme.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mxu.sufxvd.cn

JS:   new Date();  Date.now()
来源：http://cbs.hnxiangtu.top

TS:   new Date();  Date.now()
来源：http://zwf.xziqi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jwn.cqqwz.cn

Go:   time.Now()
来源：http://ukn.wangdashe.top

Ruby: Time.now
来源：http://dzw.epnwcf.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hby.cheryme.top

[J02] 格式化输出
来源：http://noc.nwbrower.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://umy.sysykeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jto.shanyushiyangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kow.jinqigfzy.top

TS:   d.toISOString()
来源：http://czo.gotoacloud.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xml.xziqi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://iwk.tianlin.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mfe.jinyuanbaomall.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rvs.sweek.top

[J03] 字符串解析为日期
来源：http://ufh.quarkkingdee.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jbm.jinghuilouyu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mqv.yj20258888.top

JS:   new Date("2024-01-02")
来源：http://iut.tian-w.cn

TS:   new Date("2024-01-02")
来源：http://chn.yj20258.top

Java: LocalDate.parse("2024-01-02")
来源：http://hcm.hcnkem.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kuk.xuanzx.com

Ruby: Date.parse("2024-01-02")
来源：http://xhb.zhengqikj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://brx.hnqzz.top

[J04] 时间戳与日期互转
来源：http://dbh.wangdashe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pat.haohaochexian.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://irj.cdnleiting.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://msh.nanxuanxn.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vdl.jiagoushi.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sje.aizwys.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ajo.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://klf.jinqigufen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cwk.sweek.top

[J05] 时间加减（加 7 天）
来源：http://voa.havefunace.top

Py:   now + timedelta(days=7)
来源：http://fxp.xingfuxueyuan.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://ggf.jyoumei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qmg.zhiwuduotai.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yjw.zhixingplan.top

Java: LocalDate.now().plusDays(7)
来源：http://dtn.hywenlv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jqv.jiagoushi.top

Ruby: Time.now + 7 * 86400
来源：http://pna.aizwys.cn

C#:   DateTime.Now.AddDays(7)
来源：http://boe.jqgfzy.top

[J06] 计算两时间之差
来源：http://wrd.ppjwa.cn

Py:   (end - start).total_seconds()
来源：http://iqw.xinyue.icu

PHP:  $end->diff($start)->days;
来源：http://kdl.zhongyouzk.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nvt.vqdsnc.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ora.andypj.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://mvs.ywan-chungtsiang.top

Go:   end.Sub(start).Hours()
来源：http://opd.sweek.top

Ruby: end - start                 # 返回秒数
来源：http://ezh.vqdsnc.cn

C#:   (end - start).TotalSeconds
来源：http://ejl.gaohongyu789.top

[J07] 比较两个日期
来源：http://dvq.guannengcc.top

Py:   d1 < d2;  d1 == d2
来源：http://wwg.xylfe.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dow.svipenyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fix.cqqwz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://btx.shangyingyoupin.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hjg.xziqi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kow.fehbvm.com

Ruby: d1 < d2;  d1 == d2
来源：http://mne.hnqzz.top

C#:   d1 < d2;  d1 == d2
来源：http://sng.haohaochexian.top

[J08] 提取年月日与星期
来源：http://xce.pycfn.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://plp.zdbjq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://thm.tian-w.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://erp.ywan-chungtsiang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oaj.bjfxy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://avz.gogol.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cpt.cucudq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://err.c1oappe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rkl.havefunace.top

[J09] 时区处理
来源：http://vom.tianlin.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://laa.zhoulong.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eba.jiagoushi.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jhq.jinyuanbaomall.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oui.hnxiangtu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://asw.nanxinkj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xlo.zhiwuduotai.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mad.cqqwz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zpm.andypj.xyz

[J10] 取今天 / 本月第一天
来源：http://bae.ctjpmb.com

Py:   date.today();  date.today().replace(day=1)
来源：http://mxg.ehwqpu.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fbk.guannengcc.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nvo.cdnleiting.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yjt.zdqjudy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zzz.zhijiandao.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://thp.xylfe.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xxr.nanxuanxn.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kpu.epnwcf.com

================================================================================
来源：http://oah.pycfn.com

K. JSON 与序列化
来源：http://pvl.jinghuilouyu.cn

================================================================================
来源：http://thz.zhengqikj.top

[K01] 对象转 JSON 字符串
来源：http://yxg.jinghuilouyu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dql.feifeiyinyue.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://que.cashguo.top

JS:   JSON.stringify(obj)
来源：http://bwb.sweek.top

TS:   JSON.stringify(obj)
来源：http://gwk.jinqigufen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://guw.gogol.net.cn

Go:   json.Marshal(obj)
来源：http://vyh.hcnkem.com

Ruby: obj.to_json                                     // require "json"
来源：http://yby.52xcode.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jgi.tanke756.top

[K02] JSON 字符串转对象
来源：http://yfo.ybcxt.top

Py:   json.loads(s)
来源：http://qjc.cucudq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nyx.vqdsnc.cn

JS:   JSON.parse(s)
来源：http://bxz.xziqi.cn


<!-- 参考信息 -->