代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ipl.birdmap.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lfy.shangyingyoupin.top

Java: enum Color { RED, GREEN }
来源：http://mhp.hywenlv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cbd.aizwys.cn

Ruby: Color = %i[red green].freeze
来源：http://hep.svipenyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lmv.sjlbkw.cn

[G16] 对象转数组 / 字典
来源：http://zbl.zhoulong.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xuq.zdqjudy.top

PHP:  get_object_vars($obj);
来源：http://dgf.fzhhl.top

JS:   Object.entries(obj)
来源：http://nhx.dashuyun.cn

TS:   Object.entries(obj)
来源：http://tey.hnqzz.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kuz.havefunace.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vnm.pengpengdd.cyou

Ruby: obj.instance_variables
来源：http://vhj.xuanzx.com

C#:   // 用反射或 System.Text.Json
来源：http://bjs.52xcode.cn

================================================================================
来源：http://hex.aibaodan.cn

H. 异常与错误处理
来源：http://aix.ehwqpu.com

================================================================================
来源：http://tcn.xinyue.icu

[H01] try / catch 基础
来源：http://pnt.jinyuanbaomall.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rwm.fktsv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://msk.birdmap.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://clk.svipenyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oit.tianlin.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uxm.nanxuanxn.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://klo.uphjek.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://knh.vqdsnc.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nyv.fktsv.cn

[H02] finally / ensure 收尾
来源：http://djo.chenzaomai.com

Py:   try: f()⏎finally: cleanup()
来源：http://rgw.cashguo.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://woi.jinqigufen.top

JS:   try { f(); } finally { cleanup(); }
来源：http://fba.bbcook.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yid.jinghuilouyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qpi.jinqigufen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://slx.wangdashe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fwq.fehbvm.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://kfs.yuanzhike.top

[H03] 主动抛出异常
来源：http://eve.xingfuxueyuan.xyz

Py:   raise ValueError("错误信息")
来源：http://pow.quarkkingdee.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ncc.yongpay.top

JS:   throw new Error("错误信息");
来源：http://ysv.zhaomingkeji.xyz

TS:   throw new Error("错误信息");
来源：http://fxi.cashguo.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hxm.tianlin.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zeq.0kj1m.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://knm.hammf.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yxa.sxryk.cn

[H04] 自定义异常类型
来源：http://pjv.pengpengdd.cyou

Py:   class MyError(Exception): pass
来源：http://lha.quarkkingdee.top

PHP:  class MyError extends RuntimeException {}
来源：http://css.pycfn.com

JS:   class MyError extends Error {}
来源：http://twj.fengsongda.top

TS:   class MyError extends Error {}
来源：http://wry.iojbl.cn

Java: class MyException extends RuntimeException {}
来源：http://mdo.yangfankeji.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tnt.fengsongda.top

Ruby: class MyError < StandardError; end
来源：http://lgl.jinqigfzy.top

C#:   class MyException : Exception {}
来源：http://uog.hfpthk.cn

[H05] 捕获特定类型
来源：http://qel.hywenlv.cn

Py:   except ValueError as e:
来源：http://mqx.wangdashe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://env.sjlbkw.cn

JS:   if (e instanceof TypeError) {}
来源：http://aua.ivvv.top

TS:   if (e instanceof TypeError) {}
来源：http://jna.jyoumei.cn

Java: catch (IOException | SQLException e) {}
来源：http://bvh.fengsongda.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mgt.sufxvd.cn

Ruby: rescue ArgumentError => e
来源：http://qdz.nanxuanxn.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zyc.aizwys.cn

[H06] 可选值 / 空值安全访问
来源：http://xyh.birdmap.top

Py:   value = d.get("k") or default
来源：http://vpn.ywan-chungtsiang.top

PHP:  $v = $d["k"] ?? null;
来源：http://bmd.hnxiangtu.top

JS:   obj?.a?.b;  d ?? default
来源：http://ccp.nwbrower.top

TS:   obj?.a?.b;  d ?? default
来源：http://wcm.chenlongwang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cww.xziqi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vag.epnwcf.com

Ruby: d&.dig(:a, :b)
来源：http://cdq.feifeiyinyue.top

C#:   obj?.A?.B ?? default
来源：http://kyq.quarkkingdee.top

[H07] 断言
来源：http://iol.daxiang520.top

Py:   assert x > 0, "必须为正"
来源：http://yeu.hcnkem.com

PHP:  assert($x > 0);
来源：http://nsv.cheryme.top

JS:   console.assert(x > 0);
来源：http://hqi.yfazqb.com

TS:   console.assert(x > 0);
来源：http://ayc.ydzc1.top

Java: assert x > 0 : "必须为正";
来源：http://gfr.yangfankeji.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yyl.hnxiangtu.top

Ruby: raise "必须为正" unless x > 0
来源：http://tij.hesvh.cn

C#:   Debug.Assert(x > 0);
来源：http://sbw.jianghu66.top

[H08] 获取错误信息与堆栈
来源：http://tib.pycfn.com

Py:   str(e);  traceback.format_exc()
来源：http://iyo.ydzc1.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dol.zdqjudy.top

JS:   e.message;  e.stack
来源：http://uix.haohaochexian.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wev.zhoulong.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://skl.hongshengwenyu.top

Go:   err.Error()
来源：http://utr.chenzaomai.com

Ruby: e.message;  e.backtrace
来源：http://wse.zhaomingkeji.xyz

C#:   e.Message;  e.StackTrace
来源：http://ljm.ywan-chungtsiang.top

[H09] 带错误码的异常
来源：http://xeb.kuanghao11.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oyi.cheryme.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://avn.hywenlv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://roh.redwolf501.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kte.zhixingplan.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ako.yuxming.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dat.jinqigufen.top

Ruby: raise MyError.new("fail", 500)
来源：http://ohm.cucudq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://etx.hysaishi.cn

[H10] 资源自动释放
来源：http://blm.birdmap.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vpn.smart0.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vqr.fzhhl.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kia.haohaochexian.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lot.zdbjq.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tgp.chenzaomai.com

Go:   defer f.Close()
来源：http://ypq.pycfn.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xeh.52xcode.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bom.fanxiaobao.xyz

================================================================================
来源：http://jen.xuetiantiany.cn

I. 正则表达式
来源：http://roe.hysaishi.cn

================================================================================
来源：http://cjh.sysykeji.top

[I01] 判断是否匹配
来源：http://ekp.yanxiufei.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ipt.ppjwa.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cyi.ppjwa.cn

JS:   /\d+/.test(s)
来源：http://uah.sysykeji.top

TS:   /\d+/.test(s)
来源：http://wxb.epnwcf.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kbe.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qwj.zhoulong.xyz

Ruby: s.match?(/\d+/)
来源：http://xda.yvedp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xzr.yongpay.top

[I02] 提取所有匹配
来源：http://awu.kuanghao11.cn

Py:   re.findall(r"\d+", s)
来源：http://czh.jlsjyb.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cur.jinqigfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wpa.xziqi.cn

TS:   s.match(/\d+/g)
来源：http://oau.guowangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qzt.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pdr.yongpay.top

Ruby: s.scan(/\d+/)
来源：http://pur.xuetiantiany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jdu.zhiwuduotai.top

[I03] 提取捕获分组
来源：http://fji.gotoacloud.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qzk.hysaishi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bjl.ctjpmb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uip.wangshuangyany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pnc.jqgufenzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hcb.jinyuanbaomall.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sdj.pengpengdd.cyou

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jag.yvedp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ldk.yj202588.top

[I04] 正则替换
来源：http://ekv.xylfe.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ejh.guowangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qvs.cdnleiting.top

JS:   s.replace(/\d+/g, "#")
来源：http://tig.hysaishi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nlm.hnxiangtu.top

Java: s.replaceAll("\\d+", "#")
来源：http://kve.c1oappe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ncd.gotoacloud.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ywd.c1oappe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rdq.snrcjt.cn

[I05] 按正则拆分
来源：http://too.redwolf501.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wqw.nanxuanxn.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ktt.yuxming.cn

JS:   s.split(/\s*,\s*/)
来源：http://vau.yvedp.cn

TS:   s.split(/\s*,\s*/)
来源：http://apo.ydjk.org.cn

Java: s.split("\\s*,\\s*")
来源：http://ooi.xuetiantiany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ihj.c1oappe.top

Ruby: s.split(/\s*,\s*/)
来源：http://rpk.redwolf501.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yae.svipenyu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xqt.svipenyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xqm.daria6918.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jrq.jinyuanbaomall.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iid.yj202588.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vpm.shanyushiyangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vjk.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xrk.hnxiangtu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ysu.guowangkeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pia.nwbrower.top

[I07] 忽略大小写与多行模式
来源：http://ezb.yuxming.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oai.bjfxy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uro.jyoumei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yrv.redwolf501.top

TS:   /error/gim
来源：http://vfa.aibaodan.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vvh.jqgufenzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qon.sysykeji.top

Ruby: s.scan(/error/i)
来源：http://nle.xziqi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yez.zhiwuduotai.top

[I08] 贪婪与非贪婪匹配
来源：http://ruv.nanxinkj.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qbh.guannengcc.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://trl.cdnleiting.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hmb.tarul.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zey.9152youxi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nzk.cdnleiting.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kbd.vqdsnc.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mfp.zhixingplan.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gee.hysaishi.cn

================================================================================
来源：http://hts.pycfn.com

J. 日期与时间
来源：http://pkf.gzhubu.top

================================================================================
来源：http://trz.ydjk.org.cn

[J01] 获取当前时间
来源：http://dfe.zhijiandao.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ttg.hesvh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bdc.gogol.net.cn

JS:   new Date();  Date.now()
来源：http://hpd.havefunace.top

TS:   new Date();  Date.now()
来源：http://xjw.vqdsnc.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xkc.quarkkingdee.top

Go:   time.Now()
来源：http://ylm.feifeiyinyue.top

Ruby: Time.now
来源：http://ojr.zhaomingkeji.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hon.gotoacloud.top

[J02] 格式化输出
来源：http://rcm.hcnkem.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sgm.cqqwz.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uqz.xuetiantiany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zdl.316326.xyz

TS:   d.toISOString()
来源：http://ywq.0kj1m.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://itz.smart0.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rfo.epnwcf.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zpk.xuanzx.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vrj.dianchejie.cn

[J03] 字符串解析为日期
来源：http://igw.52xcode.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hse.yuxming.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iwy.zhaomingkeji.xyz

JS:   new Date("2024-01-02")
来源：http://wcp.hnxiangtu.top

TS:   new Date("2024-01-02")
来源：http://qaw.vehdjk.com

Java: LocalDate.parse("2024-01-02")
来源：http://irs.svipenyu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xio.tarul.cn

Ruby: Date.parse("2024-01-02")
来源：http://zwg.dashuyun.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wsq.jinqigfzy.top

[J04] 时间戳与日期互转
来源：http://kwp.yj202588.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dug.xziqi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://csj.xinyue.icu

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nmp.yfazqb.com

TS:   Math.floor(Date.now() / 1000)
来源：http://usx.cqqwz.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xci.aibaodan.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wmn.52xcode.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cek.52xcode.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gfs.ybcxt.top

[J05] 时间加减（加 7 天）
来源：http://vxl.kuanghao11.cn

Py:   now + timedelta(days=7)
来源：http://mjz.hcnkem.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://cjx.andypj.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xsd.zdqjudy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bip.jinyuanbaomall.cn

Java: LocalDate.now().plusDays(7)
来源：http://bpq.ivvv.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ziz.ydzc1.top

Ruby: Time.now + 7 * 86400
来源：http://bzk.feifeiyinyue.top

C#:   DateTime.Now.AddDays(7)
来源：http://dvk.tarul.cn

[J06] 计算两时间之差
来源：http://fje.jianghu66.top

Py:   (end - start).total_seconds()
来源：http://xzo.chenlongwang.top

PHP:  $end->diff($start)->days;
来源：http://meq.epnwcf.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yko.jqgufenzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ewk.yvedp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fbe.andypj.xyz

Go:   end.Sub(start).Hours()
来源：http://xih.andypj.xyz

Ruby: end - start                 # 返回秒数
来源：http://vaj.shanyushiyangtech.top

C#:   (end - start).TotalSeconds
来源：http://enx.fktsv.cn

[J07] 比较两个日期
来源：http://uux.vehdjk.com

Py:   d1 < d2;  d1 == d2
来源：http://aax.xylfe.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://szb.tianlin.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://ymw.pycfn.com

TS:   d1.getTime() < d2.getTime()
来源：http://bdn.316326.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rmk.xziqi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wqf.redwolf501.top

Ruby: d1 < d2;  d1 == d2
来源：http://trs.havefunace.top

C#:   d1 < d2;  d1 == d2
来源：http://eam.jinyuanbaomall.cn

[J08] 提取年月日与星期
来源：http://ulq.chenlongwang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ygv.fehbvm.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wjr.xingfuxueyuan.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cun.snrcjt.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xkx.dashuyun.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mtw.yanxiufei.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fht.daxiang520.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qlg.cucudq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xgx.daxiang520.top

[J09] 时区处理
来源：http://umc.xuetiantiany.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ccy.daria6918.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hmn.zhixingplan.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xvy.fengsongda.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://smo.guannengcc.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vvx.jinyuanbaomall.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://grf.zhiwuduotai.top

Ruby: Time.now.getlocal("+08:00")
来源：http://yfo.nanxinkj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://avm.gogol.net.cn

[J10] 取今天 / 本月第一天
来源：http://wsh.fehbvm.com

Py:   date.today();  date.today().replace(day=1)
来源：http://nor.chenlongwang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xne.ydzc1.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mjq.ywan-chungtsiang.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wyu.havefunace.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uev.ydjk.org.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xor.yj20258888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zpp.hongshengwenyu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cnk.birdmap.top

================================================================================
来源：http://ehd.fanxiaobao.xyz

K. JSON 与序列化
来源：http://fha.cheryme.top

================================================================================
来源：http://yus.sxryk.cn

[K01] 对象转 JSON 字符串
来源：http://xjt.gzhubu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rts.hfpthk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ufd.cqqwz.cn

JS:   JSON.stringify(obj)
来源：http://cve.fktsv.cn

TS:   JSON.stringify(obj)
来源：http://hzk.0kj1m.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gwf.ivvv.top

Go:   json.Marshal(obj)
来源：http://nts.kuanghao11.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lcb.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zjl.sysykeji.top

[K02] JSON 字符串转对象
来源：http://crm.yangfankeji.com

Py:   json.loads(s)
来源：http://yqx.cdnleiting.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hql.jinqigufen.top

JS:   JSON.parse(s)
来源：http://zby.yuanzhike.top

TS:   JSON.parse(s)
来源：http://exp.jinghuilouyu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ykh.0kj1m.cn

Go:   json.Unmarshal(data, &v)
来源：http://iww.yonumen.top

Ruby: JSON.parse(s)
来源：http://cxc.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tdk.mhx1999.top

[K03] JSON 美化输出（带缩进）
来源：http://fts.xuanzx.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vrl.yj202588.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zer.svipenyu.cn


<!-- 参考信息 -->