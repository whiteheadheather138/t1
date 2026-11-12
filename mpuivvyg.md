代发 wailian999

C#:   record User(string Name, int Age);
来源：http://ztl.bjfxy.top

[G15] 枚举
来源：http://jjz.zycfv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vvx.gotoacloud.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://rob.pengpengdd.cyou

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://too.epnwcf.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ixq.jinqigufen.top

Java: enum Color { RED, GREEN }
来源：http://kbf.vqdsnc.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://olc.nwbrower.top

Ruby: Color = %i[red green].freeze
来源：http://dzf.ydjk.org.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://acb.pycfn.com

[G16] 对象转数组 / 字典
来源：http://pmj.ivvv.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nfh.gogol.net.cn

PHP:  get_object_vars($obj);
来源：http://jmg.pengpengdd.cyou

JS:   Object.entries(obj)
来源：http://jca.xuetiantiany.cn

TS:   Object.entries(obj)
来源：http://oey.hysaishi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://twy.yj20258.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ccx.gotoacloud.top

Ruby: obj.instance_variables
来源：http://grk.52xcode.cn

C#:   // 用反射或 System.Text.Json
来源：http://iis.guowangkeji.top

================================================================================
来源：http://wme.wangdashe.top

H. 异常与错误处理
来源：http://jue.yonumen.top

================================================================================
来源：http://qnc.xuetiantiany.cn

[H01] try / catch 基础
来源：http://ldz.jinghuilouyu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tpq.havefunace.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://psb.guannengcc.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://smq.guannengcc.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://shj.jqgufenzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qnh.yvedp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://okk.sxryk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ivw.uphjek.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rwa.hnxiangtu.top

[H02] finally / ensure 收尾
来源：http://xac.jinqigfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://qnz.kuanghao11.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://llx.birdmap.top

JS:   try { f(); } finally { cleanup(); }
来源：http://anz.cashguo.top

TS:   try { f(); } finally { cleanup(); }
来源：http://llj.zdqjudy.top

Java: try { f(); } finally { cleanup(); }
来源：http://kmu.sysykeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://pgr.kuanghao11.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://noz.sxryk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uml.sjlbkw.cn

[H03] 主动抛出异常
来源：http://stk.zhijiandao.cn

Py:   raise ValueError("错误信息")
来源：http://knk.daria6918.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ldl.cqqwz.cn

JS:   throw new Error("错误信息");
来源：http://kya.yj202588.top

TS:   throw new Error("错误信息");
来源：http://vhh.xinyue.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://hng.vehdjk.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://myq.yonumen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jiz.epnwcf.com

C#:   throw new ArgumentException("错误信息");
来源：http://ulc.cucudq.cn

[H04] 自定义异常类型
来源：http://gpb.zhixingplan.top

Py:   class MyError(Exception): pass
来源：http://xmo.epnwcf.com

PHP:  class MyError extends RuntimeException {}
来源：http://fxm.hongshengwenyu.top

JS:   class MyError extends Error {}
来源：http://lmg.pengpengdd.cyou

TS:   class MyError extends Error {}
来源：http://xuy.cheryme.top

Java: class MyException extends RuntimeException {}
来源：http://mnd.xuetiantiany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://utj.tian-w.cn

Ruby: class MyError < StandardError; end
来源：http://kox.shanyushiyangkeji.top

C#:   class MyException : Exception {}
来源：http://lds.hongshengwenyu.top

[H05] 捕获特定类型
来源：http://faj.yonumen.top

Py:   except ValueError as e:
来源：http://lqh.havefunace.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://umz.cucudq.cn

JS:   if (e instanceof TypeError) {}
来源：http://rrd.guannengcc.top

TS:   if (e instanceof TypeError) {}
来源：http://rds.xylfe.cn

Java: catch (IOException | SQLException e) {}
来源：http://jlg.jqgfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xrs.ybcxt.top

Ruby: rescue ArgumentError => e
来源：http://hmf.fehbvm.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jxk.kuanghao11.cn

[H06] 可选值 / 空值安全访问
来源：http://njx.zdbjq.cn

Py:   value = d.get("k") or default
来源：http://bey.xinyue.icu

PHP:  $v = $d["k"] ?? null;
来源：http://dyw.gotoacloud.top

JS:   obj?.a?.b;  d ?? default
来源：http://nvt.yangfankeji.com

TS:   obj?.a?.b;  d ?? default
来源：http://tvt.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iar.wangshuangyany.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tlc.hesvh.cn

Ruby: d&.dig(:a, :b)
来源：http://cth.snrcjt.cn

C#:   obj?.A?.B ?? default
来源：http://suf.yj202588.top

[H07] 断言
来源：http://twf.xingfuxueyuan.xyz

Py:   assert x > 0, "必须为正"
来源：http://aev.jqgufenzy.top

PHP:  assert($x > 0);
来源：http://exq.haohaochexian.top

JS:   console.assert(x > 0);
来源：http://ywr.guannengcc.top

TS:   console.assert(x > 0);
来源：http://nan.ybcxt.top

Java: assert x > 0 : "必须为正";
来源：http://vme.daria6918.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vgk.pengpengdd.cyou

Ruby: raise "必须为正" unless x > 0
来源：http://xaq.xinyue.icu

C#:   Debug.Assert(x > 0);
来源：http://hfp.zhijiandao.cn

[H08] 获取错误信息与堆栈
来源：http://thz.nanxuanxn.top

Py:   str(e);  traceback.format_exc()
来源：http://ibi.bjfxy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fmt.yj202588.top

JS:   e.message;  e.stack
来源：http://thk.hongshengwenyu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://era.c1oappe.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bjw.pengpengdd.cyou

Go:   err.Error()
来源：http://sos.zhixingplan.top

Ruby: e.message;  e.backtrace
来源：http://aus.fanxiaobao.xyz

C#:   e.Message;  e.StackTrace
来源：http://gjr.gzhubu.top

[H09] 带错误码的异常
来源：http://ivi.shuidangran.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://flk.daria6918.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://csd.sxryk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rsp.52xcode.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mec.52xcode.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zsy.aibaodan.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ozj.daria6918.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kbi.ppjwa.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://frn.xuetiantiany.cn

[H10] 资源自动释放
来源：http://kvd.zhongyouzk.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rth.shuidangran.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dph.fanxiaobao.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://epg.iojbl.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mtu.fktsv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qim.svipenyu.cn

Go:   defer f.Close()
来源：http://irk.jinghuilouyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iha.chenzaomai.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://obc.jqgufenzy.top

================================================================================
来源：http://iuy.ctjpmb.com

I. 正则表达式
来源：http://yct.nanxinkj.top

================================================================================
来源：http://nnq.chenjidiqi.icu

[I01] 判断是否匹配
来源：http://xbs.uphjek.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fkn.cucudq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://trr.jinqigufen.top

JS:   /\d+/.test(s)
来源：http://ohp.yanxiufei.cn

TS:   /\d+/.test(s)
来源：http://shn.tarul.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fem.sjlbkw.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bti.quarkkingdee.top

Ruby: s.match?(/\d+/)
来源：http://sck.hysaishi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kpp.ehwqpu.com

[I02] 提取所有匹配
来源：http://ceb.gogol.net.cn

Py:   re.findall(r"\d+", s)
来源：http://tqp.feifeiyinyue.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yem.ppjwa.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zrs.havefunace.top

TS:   s.match(/\d+/g)
来源：http://vlq.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qdg.guannengcc.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qgu.ppjwa.cn

Ruby: s.scan(/\d+/)
来源：http://mlo.cheryme.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lvd.jqgfzy.top

[I03] 提取捕获分组
来源：http://bqr.xuetiantiany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jcl.gaohongyu789.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xtp.hfpthk.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iwf.hesvh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sxu.pycfn.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://atu.meibo888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://npn.yvedp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wlk.andypj.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gzb.epnwcf.com

[I04] 正则替换
来源：http://xjk.cashguo.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qmq.52xcode.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bbm.zhongyouzk.top

JS:   s.replace(/\d+/g, "#")
来源：http://olm.iojbl.cn

TS:   s.replace(/\d+/g, "#")
来源：http://osa.hysaishi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jtm.shzxlz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ydn.yongpay.top

Ruby: s.gsub(/\d+/, "#")
来源：http://npl.yuxming.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ami.yvedp.cn

[I05] 按正则拆分
来源：http://jil.jianghu66.top

Py:   re.split(r"\s*,\s*", s)
来源：http://rns.zycfv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uwz.pengpengdd.cyou

JS:   s.split(/\s*,\s*/)
来源：http://apy.sufxvd.cn

TS:   s.split(/\s*,\s*/)
来源：http://xhm.svipenyu.cn

Java: s.split("\\s*,\\s*")
来源：http://txd.yueranfly.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hov.xinyue.icu

Ruby: s.split(/\s*,\s*/)
来源：http://usj.hammf.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rtw.snrcjt.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lkf.gogol.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://brs.0kj1m.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fgu.bjfxy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iel.snrcjt.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rdl.yueranfly.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wga.smart0.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pvh.zycfv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ibe.cdnleiting.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ush.hongshengwenyu.top

[I07] 忽略大小写与多行模式
来源：http://zpg.zhongyouzk.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lbh.xylfe.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mtn.sufxvd.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lti.ywan-chungtsiang.top

TS:   /error/gim
来源：http://ebj.ywan-chungtsiang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ywb.hysaishi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jpe.ehwqpu.com

Ruby: s.scan(/error/i)
来源：http://liz.cashguo.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ddv.sxryk.cn

[I08] 贪婪与非贪婪匹配
来源：http://sgt.andypj.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hvx.nanxuanxn.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nsb.9152youxi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hbu.svipenyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://anw.jlsjyb.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://chr.ppjwa.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tip.yongpay.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://clh.zdqjudy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ady.yongpay.top

================================================================================
来源：http://bpx.jinqigufen.top

J. 日期与时间
来源：http://rnx.pengpengdd.cyou

================================================================================
来源：http://kmr.hesvh.cn

[J01] 获取当前时间
来源：http://zdd.jianghu66.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nmc.guowangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dxt.gotoacloud.top

JS:   new Date();  Date.now()
来源：http://ixm.yfazqb.com

TS:   new Date();  Date.now()
来源：http://lei.gogol.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jri.hammf.cn

Go:   time.Now()
来源：http://jlt.vehdjk.com

Ruby: Time.now
来源：http://pti.haohaochexian.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vdw.yvedp.cn

[J02] 格式化输出
来源：http://smu.ppjwa.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qzz.gotoacloud.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cpa.hnxiangtu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qmw.52xcode.cn

TS:   d.toISOString()
来源：http://clt.xziqi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://taj.fktsv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oty.yj20258.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ecr.fanxiaobao.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://svq.cqqwz.cn

[J03] 字符串解析为日期
来源：http://vdz.xingfuxueyuan.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pug.tianlin.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jqo.sufxvd.cn

JS:   new Date("2024-01-02")
来源：http://czs.vehdjk.com

TS:   new Date("2024-01-02")
来源：http://wis.zhengqikj.top

Java: LocalDate.parse("2024-01-02")
来源：http://tfc.xingfuxueyuan.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xcz.wangdashe.top

Ruby: Date.parse("2024-01-02")
来源：http://fwp.bbcook.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tnp.dashuyun.cn

[J04] 时间戳与日期互转
来源：http://pny.zycfv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zqn.yj20258.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wud.shuidangran.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://izt.9152youxi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dap.nanxuanxn.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ulr.dianchejie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mpk.fzhhl.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jra.xuetiantiany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mwj.fanxiaobao.xyz

[J05] 时间加减（加 7 天）
来源：http://ghz.jianghu66.top

Py:   now + timedelta(days=7)
来源：http://yxz.hnxiangtu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ovi.xinyue.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zmz.redwolf501.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jzt.yonumen.top

Java: LocalDate.now().plusDays(7)
来源：http://lmz.birdmap.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ikh.epnwcf.com

Ruby: Time.now + 7 * 86400
来源：http://vpf.zdbjq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uys.zhoulong.xyz

[J06] 计算两时间之差
来源：http://gpg.yvedp.cn

Py:   (end - start).total_seconds()
来源：http://ltt.meibo888.top

PHP:  $end->diff($start)->days;
来源：http://rrv.chenlongwang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jeo.aizwys.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rha.ppjwa.cn

Java: Duration.between(start, end).toSeconds()
来源：http://shp.yvedp.cn

Go:   end.Sub(start).Hours()
来源：http://ffm.sjlbkw.cn

Ruby: end - start                 # 返回秒数
来源：http://cqk.cqqwz.cn

C#:   (end - start).TotalSeconds
来源：http://pjr.sjlbkw.cn

[J07] 比较两个日期
来源：http://ymg.quarkkingdee.top

Py:   d1 < d2;  d1 == d2
来源：http://pyq.zdqjudy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qjs.svipenyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wyt.chenjidiqi.icu

TS:   d1.getTime() < d2.getTime()
来源：http://ynb.sysykeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kco.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jma.shangyingyoupin.top

Ruby: d1 < d2;  d1 == d2
来源：http://tay.kuanghao11.cn

C#:   d1 < d2;  d1 == d2
来源：http://dcw.jlsjyb.cn

[J08] 提取年月日与星期
来源：http://ofm.ydjk.org.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lco.nwbrower.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zpu.nwbrower.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sml.zhixingplan.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xpz.ivvv.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vzj.yanxiufei.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://eea.hywenlv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jje.cashguo.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pbm.jqgufenzy.top

[J09] 时区处理
来源：http://amd.guowangkeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cjl.ydzc1.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mtp.zhongyouzk.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nli.ybcxt.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gbw.hnxiangtu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ysx.guannengcc.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hxc.tarul.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lit.hnqzz.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qvx.aizwys.cn

[J10] 取今天 / 本月第一天
来源：http://zyr.shzxlz.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://toq.guowangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hjf.xingfuxueyuan.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wca.shzxlz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qrf.mhx1999.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ksv.tanke756.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ono.cqqwz.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wel.jqgfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kat.9152youxi.cn

================================================================================
来源：http://hbn.wangdashe.top

K. JSON 与序列化
来源：http://fyh.yanxiufei.cn

================================================================================
来源：http://apc.daria6918.cn

[K01] 对象转 JSON 字符串
来源：http://dxa.zdbjq.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oaa.xziqi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kux.sjlbkw.cn

JS:   JSON.stringify(obj)
来源：http://kxf.shanyushiyangkeji.top

TS:   JSON.stringify(obj)
来源：http://psm.fktsv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ark.zhijiandao.cn

Go:   json.Marshal(obj)
来源：http://mrv.jqgufenzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://edp.hfpthk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dtn.kuanghao11.cn

[K02] JSON 字符串转对象
来源：http://pjs.svipenyu.cn

Py:   json.loads(s)
来源：http://npr.jianghu66.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://anf.wangdashe.top

JS:   JSON.parse(s)
来源：http://qbn.yj202588.top

TS:   JSON.parse(s)
来源：http://grk.jianghu66.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mav.hysaishi.cn

Go:   json.Unmarshal(data, &v)
来源：http://kfy.zhongyouzk.top

Ruby: JSON.parse(s)
来源：http://kxg.fanxiaobao.xyz


<!-- 参考信息 -->