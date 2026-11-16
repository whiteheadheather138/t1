代发 wailian999

PHP:  get_object_vars($obj);
来源：http://ysb.hongshengwenyu.top

JS:   Object.entries(obj)
来源：http://ulf.fzhhl.top

TS:   Object.entries(obj)
来源：http://cjx.hesvh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://snb.iojbl.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bqu.ydjk.org.cn

Ruby: obj.instance_variables
来源：http://qvh.c1oappe.top

C#:   // 用反射或 System.Text.Json
来源：http://zoe.zhixingplan.top

================================================================================
来源：http://kic.feifeiyinyue.top

H. 异常与错误处理
来源：http://yex.jinyuanbaomall.cn

================================================================================
来源：http://ywy.tarul.cn

[H01] try / catch 基础
来源：http://hsq.cdnleiting.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qws.jianghu66.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gey.jianghu66.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gpj.zhixingplan.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://doc.hywenlv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uru.hnxiangtu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qnr.snrcjt.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://azk.yj20258.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yvw.daxiang520.top

[H02] finally / ensure 收尾
来源：http://agg.sysykeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://fgo.jinyuanbaomall.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lpb.jinghuilouyu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://chj.tian-w.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cvn.shanyushiyangtech.top

Java: try { f(); } finally { cleanup(); }
来源：http://vba.chenlongwang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mqr.tian-w.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://eas.vqdsnc.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://atd.hammf.cn

[H03] 主动抛出异常
来源：http://dyv.9152youxi.cn

Py:   raise ValueError("错误信息")
来源：http://wwx.zdbjq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://aqu.yongpay.top

JS:   throw new Error("错误信息");
来源：http://dho.yj202588.top

TS:   throw new Error("错误信息");
来源：http://mex.gotoacloud.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jgi.zhengqikj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hzw.yvedp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fqb.sjlbkw.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wvz.vqdsnc.cn

[H04] 自定义异常类型
来源：http://jze.zhongyouzk.top

Py:   class MyError(Exception): pass
来源：http://eub.zhongyouzk.top

PHP:  class MyError extends RuntimeException {}
来源：http://giy.guowangkeji.top

JS:   class MyError extends Error {}
来源：http://qqu.cashguo.top

TS:   class MyError extends Error {}
来源：http://yth.cqqwz.cn

Java: class MyException extends RuntimeException {}
来源：http://jyc.hnqzz.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yqz.havefunace.top

Ruby: class MyError < StandardError; end
来源：http://ihv.haohaochexian.top

C#:   class MyException : Exception {}
来源：http://lyc.zhiwuduotai.top

[H05] 捕获特定类型
来源：http://jcn.52xcode.cn

Py:   except ValueError as e:
来源：http://txs.quarkkingdee.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nvp.jianghu66.top

JS:   if (e instanceof TypeError) {}
来源：http://sia.zhoulong.xyz

TS:   if (e instanceof TypeError) {}
来源：http://gsg.dashuyun.cn

Java: catch (IOException | SQLException e) {}
来源：http://eko.ywan-chungtsiang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wet.daria6918.cn

Ruby: rescue ArgumentError => e
来源：http://lpb.ctjpmb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ttu.chenlongwang.top

[H06] 可选值 / 空值安全访问
来源：http://gty.sysykeji.top

Py:   value = d.get("k") or default
来源：http://wwi.hysaishi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lus.vehdjk.com

JS:   obj?.a?.b;  d ?? default
来源：http://lno.iojbl.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jxn.nanxuanxn.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rta.xuetiantiany.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fgh.sjlbkw.cn

Ruby: d&.dig(:a, :b)
来源：http://iwy.yonumen.top

C#:   obj?.A?.B ?? default
来源：http://gub.guannengcc.top

[H07] 断言
来源：http://sau.epnwcf.com

Py:   assert x > 0, "必须为正"
来源：http://oyi.mhx1999.top

PHP:  assert($x > 0);
来源：http://ddy.zdqjudy.top

JS:   console.assert(x > 0);
来源：http://vid.birdmap.top

TS:   console.assert(x > 0);
来源：http://kby.cucudq.cn

Java: assert x > 0 : "必须为正";
来源：http://ylb.cdnleiting.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rra.shzxlz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kla.ydjk.org.cn

C#:   Debug.Assert(x > 0);
来源：http://bnt.yj202588.top

[H08] 获取错误信息与堆栈
来源：http://khr.xingfuxueyuan.xyz

Py:   str(e);  traceback.format_exc()
来源：http://uht.gotoacloud.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qnv.dashuyun.cn

JS:   e.message;  e.stack
来源：http://rbu.tianlin.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://khg.kuanghao11.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://adf.wangshuangyany.cn

Go:   err.Error()
来源：http://trc.sxryk.cn

Ruby: e.message;  e.backtrace
来源：http://tjv.hnqzz.top

C#:   e.Message;  e.StackTrace
来源：http://rbu.vqdsnc.cn

[H09] 带错误码的异常
来源：http://dxg.shzxlz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://owk.aibaodan.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://laf.fzhhl.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qfb.sjlbkw.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://idu.wangshuangyany.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ibl.zhaomingkeji.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jcy.zhoulong.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://ztj.gogol.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pau.xuanzx.com

[H10] 资源自动释放
来源：http://tgg.birdmap.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://avo.fanxiaobao.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xfd.ywan-chungtsiang.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://obz.xingfuxueyuan.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iib.ybcxt.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oav.zdqjudy.top

Go:   defer f.Close()
来源：http://ved.hnxiangtu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zln.yj20258888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hwq.vqdsnc.cn

================================================================================
来源：http://nzr.yj20258.top

I. 正则表达式
来源：http://mew.cqqwz.cn

================================================================================
来源：http://yam.jqgufenzy.top

[I01] 判断是否匹配
来源：http://psj.zhiwuduotai.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://stv.mhx1999.top

PHP:  preg_match('/\d+/', $s);
来源：http://twj.ppjwa.cn

JS:   /\d+/.test(s)
来源：http://jmk.andypj.xyz

TS:   /\d+/.test(s)
来源：http://boi.shuidangran.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qux.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mxg.wangdashe.top

Ruby: s.match?(/\d+/)
来源：http://kwf.hysaishi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uby.yj202588.top

[I02] 提取所有匹配
来源：http://aky.hnxiangtu.top

Py:   re.findall(r"\d+", s)
来源：http://mpm.c1oappe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lgm.hnxiangtu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://suh.shangyingyoupin.top

TS:   s.match(/\d+/g)
来源：http://geg.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xmm.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vhc.sufxvd.cn

Ruby: s.scan(/\d+/)
来源：http://bgq.chenjidiqi.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lql.nwbrower.top

[I03] 提取捕获分组
来源：http://jpi.xziqi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kuv.fzhhl.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hpo.zhiwuduotai.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mcg.dashuyun.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ffw.haohaochexian.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tqg.svipenyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nfe.tarul.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iyh.shzxlz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xze.52xcode.cn

[I04] 正则替换
来源：http://vip.hysaishi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vch.hnqzz.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zxc.hysaishi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://adk.cucudq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ael.xingfuxueyuan.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://ipv.xinyue.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://zxf.yanxiufei.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hrb.ydzc1.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://smq.yj202588.top

[I05] 按正则拆分
来源：http://gyh.yangfankeji.com

Py:   re.split(r"\s*,\s*", s)
来源：http://pvl.jqgfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rwp.daxiang520.top

JS:   s.split(/\s*,\s*/)
来源：http://eec.hammf.cn

TS:   s.split(/\s*,\s*/)
来源：http://xqo.hywenlv.cn

Java: s.split("\\s*,\\s*")
来源：http://acl.ydzc1.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vwx.cheryme.top

Ruby: s.split(/\s*,\s*/)
来源：http://uny.yongpay.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vxh.hywenlv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dmi.gotoacloud.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vct.wangshuangyany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gft.guowangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://per.c1oappe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ksn.mhx1999.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ubc.ivvv.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dwc.tarul.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zbu.chenlongwang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tpk.wangdashe.top

[I07] 忽略大小写与多行模式
来源：http://uyr.daria6918.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cpo.hysaishi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://euo.guowangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wkr.316326.xyz

TS:   /error/gim
来源：http://jhg.aibaodan.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hdr.haohaochexian.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zsn.fzhhl.top

Ruby: s.scan(/error/i)
来源：http://mrw.yj20258.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uex.tanke756.top

[I08] 贪婪与非贪婪匹配
来源：http://xxl.yj202588.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ihd.yj20258.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hrf.wangdashe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mng.hysaishi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kyy.shzxlz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jgt.shanyushiyangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://abf.yuxming.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wdz.0kj1m.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zov.snrcjt.cn

================================================================================
来源：http://qlh.fktsv.cn

J. 日期与时间
来源：http://rlb.shanyushiyangkeji.top

================================================================================
来源：http://shq.jinyuanbaomall.cn

[J01] 获取当前时间
来源：http://xko.ehwqpu.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://jov.chenzaomai.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qok.daxiang520.top

JS:   new Date();  Date.now()
来源：http://gau.aizwys.cn

TS:   new Date();  Date.now()
来源：http://cmr.kuanghao11.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ewp.jinyuanbaomall.cn

Go:   time.Now()
来源：http://liy.daxiang520.top

Ruby: Time.now
来源：http://pkp.nanxuanxn.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://znj.zdqjudy.top

[J02] 格式化输出
来源：http://hew.yongpay.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nfa.cheryme.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hki.sweek.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nom.smart0.xyz

TS:   d.toISOString()
来源：http://lsl.yj202588.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mqf.hcnkem.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yjr.wangshuangyany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cvn.wangshuangyany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dkb.sweek.top

[J03] 字符串解析为日期
来源：http://dgd.xuanzx.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pyb.jinghuilouyu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fcc.yj20258888.top

JS:   new Date("2024-01-02")
来源：http://xpi.jinyuanbaomall.cn

TS:   new Date("2024-01-02")
来源：http://foc.quarkkingdee.top

Java: LocalDate.parse("2024-01-02")
来源：http://wol.cqqwz.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nxg.hywenlv.cn

Ruby: Date.parse("2024-01-02")
来源：http://cdb.chenjidiqi.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qjr.pengpengdd.cyou

[J04] 时间戳与日期互转
来源：http://krh.nanxinkj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://miu.yj202588.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xms.jinghuilouyu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vks.yfazqb.com

TS:   Math.floor(Date.now() / 1000)
来源：http://iuu.tanke756.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aik.yueranfly.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://edx.jinghuilouyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gcp.yuanzhike.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eli.52xcode.cn

[J05] 时间加减（加 7 天）
来源：http://xpl.zhongyouzk.top

Py:   now + timedelta(days=7)
来源：http://xli.hammf.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dty.yangfankeji.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oza.zhoulong.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gxj.zhaomingkeji.xyz

Java: LocalDate.now().plusDays(7)
来源：http://dpi.zdqjudy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ufa.tianlin.xyz

Ruby: Time.now + 7 * 86400
来源：http://bqp.yangfankeji.com

C#:   DateTime.Now.AddDays(7)
来源：http://xzd.wangdashe.top

[J06] 计算两时间之差
来源：http://ibd.yfazqb.com

Py:   (end - start).total_seconds()
来源：http://soi.fengsongda.top

PHP:  $end->diff($start)->days;
来源：http://iak.shanyushiyangtech.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gdf.uphjek.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://umo.yueranfly.top

Java: Duration.between(start, end).toSeconds()
来源：http://dbg.smart0.xyz

Go:   end.Sub(start).Hours()
来源：http://zrp.nanxinkj.top

Ruby: end - start                 # 返回秒数
来源：http://qfs.ywan-chungtsiang.top

C#:   (end - start).TotalSeconds
来源：http://nzw.zdqjudy.top

[J07] 比较两个日期
来源：http://ygg.hywenlv.cn

Py:   d1 < d2;  d1 == d2
来源：http://feo.jqgfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cmq.ctjpmb.com

JS:   d1.getTime() < d2.getTime()
来源：http://xxp.haohaochexian.top

TS:   d1.getTime() < d2.getTime()
来源：http://vwn.aizwys.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://koh.guowangkeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wyd.vehdjk.com

Ruby: d1 < d2;  d1 == d2
来源：http://nno.epnwcf.com

C#:   d1 < d2;  d1 == d2
来源：http://jjw.aizwys.cn

[J08] 提取年月日与星期
来源：http://ufo.yuanzhike.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mcg.sysykeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://egr.fktsv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vmq.hfpthk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vfr.cashguo.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uhv.zhaomingkeji.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://chy.tanke756.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tai.xuanzx.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pqv.kuanghao11.cn

[J09] 时区处理
来源：http://qbi.jqgufenzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mzu.shzxlz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nhe.jqgfzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jgq.svipenyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rhe.jqgufenzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ldp.shanyushiyangtech.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gid.havefunace.top

Ruby: Time.now.getlocal("+08:00")
来源：http://rat.tian-w.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xfq.yueranfly.top

[J10] 取今天 / 本月第一天
来源：http://xvg.hammf.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://aej.uphjek.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nxj.xuanzx.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ttb.ehwqpu.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yqd.yuxming.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lpl.hysaishi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gns.cdnleiting.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ldf.fanxiaobao.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bgm.tianlin.xyz

================================================================================
来源：http://gip.yuxming.cn

K. JSON 与序列化
来源：http://pao.chenzaomai.com

================================================================================
来源：http://nrg.sufxvd.cn

[K01] 对象转 JSON 字符串
来源：http://tya.ywan-chungtsiang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://heb.uphjek.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://chs.hcnkem.com

JS:   JSON.stringify(obj)
来源：http://iuj.fehbvm.com

TS:   JSON.stringify(obj)
来源：http://mdb.sxryk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gvd.jinghuilouyu.cn

Go:   json.Marshal(obj)
来源：http://cgp.gzhubu.top

Ruby: obj.to_json                                     // require "json"
来源：http://exe.yj20258888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://acf.c1oappe.top

[K02] JSON 字符串转对象
来源：http://sbw.epnwcf.com

Py:   json.loads(s)
来源：http://zan.fanxiaobao.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jnt.zhaomingkeji.xyz

JS:   JSON.parse(s)
来源：http://sai.andypj.xyz

TS:   JSON.parse(s)
来源：http://kux.0kj1m.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vmv.cdnleiting.top

Go:   json.Unmarshal(data, &v)
来源：http://vwr.havefunace.top

Ruby: JSON.parse(s)
来源：http://wxj.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dhv.hysaishi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ees.zhongyouzk.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gpn.ivvv.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nwd.zhengqikj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://utt.pycfn.com

TS:   JSON.stringify(obj, null, 2)
来源：http://bvo.epnwcf.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xhy.mhx1999.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nhm.zhiwuduotai.top

Ruby: JSON.pretty_generate(obj)
来源：http://ifw.jqgfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lnj.zhengqikj.top

[K04] 读取 JSON 文件
来源：http://gkt.hnqzz.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cqm.gzhubu.top


<!-- 参考信息 -->