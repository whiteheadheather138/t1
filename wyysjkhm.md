代发 wailian999

PHP:  get_object_vars($obj);
来源：http://bxs.ivvv.top

JS:   Object.entries(obj)
来源：http://zka.gaohongyu789.top

TS:   Object.entries(obj)
来源：http://iac.hywenlv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ypz.sjlbkw.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yuk.yangfankeji.com

Ruby: obj.instance_variables
来源：http://wif.zycfv.cn

C#:   // 用反射或 System.Text.Json
来源：http://swf.mhx1999.top

================================================================================
来源：http://gyo.sjlbkw.cn

H. 异常与错误处理
来源：http://pbn.vehdjk.com

================================================================================
来源：http://iko.kuanghao11.cn

[H01] try / catch 基础
来源：http://vrl.ctjpmb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uzi.ppjwa.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vma.gzhubu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xyt.wangdashe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gsa.chenzaomai.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xwl.daria6918.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kly.fengsongda.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rzz.hfpthk.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pjx.yueranfly.top

[H02] finally / ensure 收尾
来源：http://fih.316326.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://zxt.yuanzhike.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://sqg.quarkkingdee.top

JS:   try { f(); } finally { cleanup(); }
来源：http://dvc.xziqi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mwc.52xcode.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qzb.aizwys.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wst.yuxming.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kmj.uphjek.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://chd.xingfuxueyuan.xyz

[H03] 主动抛出异常
来源：http://vwr.bjfxy.top

Py:   raise ValueError("错误信息")
来源：http://kza.nanxinkj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://szt.jinqigufen.top

JS:   throw new Error("错误信息");
来源：http://kdc.sjlbkw.cn

TS:   throw new Error("错误信息");
来源：http://vrb.jinqigfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://gyn.pengpengdd.cyou

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uyx.zhaomingkeji.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://pik.jqgufenzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://qqq.0kj1m.cn

[H04] 自定义异常类型
来源：http://dxg.snrcjt.cn

Py:   class MyError(Exception): pass
来源：http://vsb.tianlin.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://xlj.yvedp.cn

JS:   class MyError extends Error {}
来源：http://fci.shanyushiyangtech.top

TS:   class MyError extends Error {}
来源：http://iph.zycfv.cn

Java: class MyException extends RuntimeException {}
来源：http://pwh.aibaodan.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jcu.sufxvd.cn

Ruby: class MyError < StandardError; end
来源：http://fll.hfpthk.cn

C#:   class MyException : Exception {}
来源：http://cgc.xuanzx.com

[H05] 捕获特定类型
来源：http://eps.guannengcc.top

Py:   except ValueError as e:
来源：http://hem.iojbl.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ony.tarul.cn

JS:   if (e instanceof TypeError) {}
来源：http://xgg.shanyushiyangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://chq.bjfxy.top

Java: catch (IOException | SQLException e) {}
来源：http://slw.zhongyouzk.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bdx.hcnkem.com

Ruby: rescue ArgumentError => e
来源：http://rjn.aibaodan.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lwe.xuetiantiany.cn

[H06] 可选值 / 空值安全访问
来源：http://tfm.xziqi.cn

Py:   value = d.get("k") or default
来源：http://dic.xingfuxueyuan.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://dek.tarul.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ozm.tanke756.top

TS:   obj?.a?.b;  d ?? default
来源：http://chm.hfpthk.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gmd.jqgufenzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qeq.daria6918.cn

Ruby: d&.dig(:a, :b)
来源：http://nrv.kuanghao11.cn

C#:   obj?.A?.B ?? default
来源：http://fgv.hnqzz.top

[H07] 断言
来源：http://tru.cqqwz.cn

Py:   assert x > 0, "必须为正"
来源：http://wmn.gogol.net.cn

PHP:  assert($x > 0);
来源：http://fad.hfpthk.cn

JS:   console.assert(x > 0);
来源：http://mes.wangdashe.top

TS:   console.assert(x > 0);
来源：http://hsd.shanyushiyangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://dng.ydzc1.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kcj.zhaomingkeji.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://yes.ydzc1.top

C#:   Debug.Assert(x > 0);
来源：http://xez.tian-w.cn

[H08] 获取错误信息与堆栈
来源：http://cyl.ydjk.org.cn

Py:   str(e);  traceback.format_exc()
来源：http://zcg.shzxlz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fch.tanke756.top

JS:   e.message;  e.stack
来源：http://shr.dashuyun.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yqu.dashuyun.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vdo.yfazqb.com

Go:   err.Error()
来源：http://fki.meibo888.top

Ruby: e.message;  e.backtrace
来源：http://poa.gzhubu.top

C#:   e.Message;  e.StackTrace
来源：http://iqe.birdmap.top

[H09] 带错误码的异常
来源：http://vml.c1oappe.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qka.cashguo.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://bhe.c1oappe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vee.bjfxy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xjf.quarkkingdee.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gne.snrcjt.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://krw.jqgfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://cvs.redwolf501.top

C#:   // 自定义异常类中加 Code 属性
来源：http://sec.shzxlz.cn

[H10] 资源自动释放
来源：http://ttn.vqdsnc.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://eow.sweek.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xeq.ctjpmb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fwe.shanyushiyangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dio.yongpay.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qnq.jqgfzy.top

Go:   defer f.Close()
来源：http://fcm.yvedp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://anf.dianchejie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rud.uphjek.com

================================================================================
来源：http://pmk.zhijiandao.cn

I. 正则表达式
来源：http://fxs.redwolf501.top

================================================================================
来源：http://mur.zhixingplan.top

[I01] 判断是否匹配
来源：http://cux.zhixingplan.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bqx.tian-w.cn

PHP:  preg_match('/\d+/', $s);
来源：http://weh.ivvv.top

JS:   /\d+/.test(s)
来源：http://svw.jinghuilouyu.cn

TS:   /\d+/.test(s)
来源：http://mix.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ohg.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cyv.sweek.top

Ruby: s.match?(/\d+/)
来源：http://nuh.bjfxy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jpq.hywenlv.cn

[I02] 提取所有匹配
来源：http://ksa.cdnleiting.top

Py:   re.findall(r"\d+", s)
来源：http://keu.bbcook.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wst.tarul.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pww.havefunace.top

TS:   s.match(/\d+/g)
来源：http://afi.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xfm.yj20258.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wpr.sjlbkw.cn

Ruby: s.scan(/\d+/)
来源：http://hxm.wangshuangyany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uth.yuxming.cn

[I03] 提取捕获分组
来源：http://gjs.ivvv.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dvs.jqgufenzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jkd.316326.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://okj.chenlongwang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vdt.smart0.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oaa.jinghuilouyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dao.nanxuanxn.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ppp.yongpay.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tnf.cqqwz.cn

[I04] 正则替换
来源：http://otu.feifeiyinyue.top

Py:   re.sub(r"\d+", "#", s)
来源：http://csk.0kj1m.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wfx.shanyushiyangtech.top

JS:   s.replace(/\d+/g, "#")
来源：http://ihy.9152youxi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zse.meibo888.top

Java: s.replaceAll("\\d+", "#")
来源：http://kzf.feifeiyinyue.top

Go:   re.ReplaceAllString(s, "#")
来源：http://nns.tian-w.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ace.ctjpmb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ceb.ywan-chungtsiang.top

[I05] 按正则拆分
来源：http://hgl.tianlin.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://art.kuanghao11.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jlf.bbcook.cn

JS:   s.split(/\s*,\s*/)
来源：http://xtz.ehwqpu.com

TS:   s.split(/\s*,\s*/)
来源：http://cqi.yuxming.cn

Java: s.split("\\s*,\\s*")
来源：http://hfu.yvedp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tun.daria6918.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nnh.yfazqb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://khx.gaohongyu789.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vfm.cucudq.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dlp.redwolf501.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ald.yj20258.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nzo.quarkkingdee.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fkz.fzhhl.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dtn.shzxlz.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zpg.wangshuangyany.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ttu.nanxuanxn.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ueu.pycfn.com

[I07] 忽略大小写与多行模式
来源：http://wab.nanxinkj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mdz.sweek.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jte.jianghu66.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ofg.jiagoushi.top

TS:   /error/gim
来源：http://ben.fanxiaobao.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wkb.sufxvd.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xgf.kuanghao11.cn

Ruby: s.scan(/error/i)
来源：http://efp.fehbvm.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qnz.xylfe.cn

[I08] 贪婪与非贪婪匹配
来源：http://qnq.zhaomingkeji.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pgw.tarul.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://crx.daria6918.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://byt.tianlin.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wuf.aizwys.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mwb.yonumen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dte.chenzaomai.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uvj.sufxvd.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yhi.hesvh.cn

================================================================================
来源：http://zyi.yvedp.cn

J. 日期与时间
来源：http://rui.daxiang520.top

================================================================================
来源：http://kca.shanyushiyangtech.top

[J01] 获取当前时间
来源：http://sml.smart0.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://boi.zdbjq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ywz.sufxvd.cn

JS:   new Date();  Date.now()
来源：http://vjo.nwbrower.top

TS:   new Date();  Date.now()
来源：http://sag.chenlongwang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://afj.dianchejie.cn

Go:   time.Now()
来源：http://xqq.cashguo.top

Ruby: Time.now
来源：http://ode.meibo888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://btu.xylfe.cn

[J02] 格式化输出
来源：http://vfx.jinqigfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ufe.sjlbkw.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tzd.ctjpmb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uhi.sysykeji.top

TS:   d.toISOString()
来源：http://ktq.chenlongwang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qjr.sxryk.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://prz.zhiwuduotai.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uyn.guannengcc.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://smx.jqgufenzy.top

[J03] 字符串解析为日期
来源：http://cgc.shanyushiyangtech.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yim.yj20258.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zkv.shanyushiyangtech.top

JS:   new Date("2024-01-02")
来源：http://xkp.chenjidiqi.icu

TS:   new Date("2024-01-02")
来源：http://anq.yueranfly.top

Java: LocalDate.parse("2024-01-02")
来源：http://auh.pycfn.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://edw.jinqigfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://ewx.tianlin.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tul.aibaodan.cn

[J04] 时间戳与日期互转
来源：http://bvk.yj202588.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hng.zhongyouzk.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jwr.0kj1m.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wlz.pengpengdd.cyou

TS:   Math.floor(Date.now() / 1000)
来源：http://wjk.shangyingyoupin.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cox.hammf.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rjr.vqdsnc.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://krb.aibaodan.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tqp.zdbjq.cn

[J05] 时间加减（加 7 天）
来源：http://fue.nanxuanxn.top

Py:   now + timedelta(days=7)
来源：http://pkm.dianchejie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ezc.hywenlv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ryg.sxryk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vwb.xziqi.cn

Java: LocalDate.now().plusDays(7)
来源：http://yea.jinqigufen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fof.xuanzx.com

Ruby: Time.now + 7 * 86400
来源：http://gmq.xingfuxueyuan.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://ihk.yongpay.top

[J06] 计算两时间之差
来源：http://wjx.birdmap.top

Py:   (end - start).total_seconds()
来源：http://twh.wangshuangyany.cn

PHP:  $end->diff($start)->days;
来源：http://dwr.jinqigfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qcp.jianghu66.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ucs.jinyuanbaomall.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sza.jqgufenzy.top

Go:   end.Sub(start).Hours()
来源：http://yfe.fktsv.cn

Ruby: end - start                 # 返回秒数
来源：http://kyd.yj20258888.top

C#:   (end - start).TotalSeconds
来源：http://umk.zhengqikj.top

[J07] 比较两个日期
来源：http://ion.nwbrower.top

Py:   d1 < d2;  d1 == d2
来源：http://xzq.shanyushiyangtech.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zhu.daria6918.cn

JS:   d1.getTime() < d2.getTime()
来源：http://csl.fengsongda.top

TS:   d1.getTime() < d2.getTime()
来源：http://eni.jlsjyb.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bqq.wangshuangyany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jza.xziqi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wqp.nwbrower.top

C#:   d1 < d2;  d1 == d2
来源：http://yjy.jinghuilouyu.cn

[J08] 提取年月日与星期
来源：http://jgt.yueranfly.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oaa.hnqzz.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sme.fengsongda.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xtb.sxryk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://esi.yfazqb.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wgm.snrcjt.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xql.tarul.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fib.nanxuanxn.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zuo.yuxming.cn

[J09] 时区处理
来源：http://gvr.chenlongwang.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://llv.yuanzhike.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xwa.zhoulong.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cbp.aibaodan.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ujr.xylfe.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xxu.52xcode.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yjr.iojbl.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://iir.aibaodan.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://crz.yfazqb.com

[J10] 取今天 / 本月第一天
来源：http://uhk.wangshuangyany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://npq.gotoacloud.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://afz.aibaodan.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://igq.sysykeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://inv.ppjwa.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hdy.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ptt.jlsjyb.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jkh.smart0.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fwc.yj202588.top

================================================================================
来源：http://fdg.9152youxi.cn

K. JSON 与序列化
来源：http://txw.bbcook.cn

================================================================================
来源：http://alc.ppjwa.cn

[K01] 对象转 JSON 字符串
来源：http://fvl.hnxiangtu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nhl.fanxiaobao.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://prj.ctjpmb.com

JS:   JSON.stringify(obj)
来源：http://qfh.jlsjyb.cn

TS:   JSON.stringify(obj)
来源：http://bfh.vqdsnc.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lol.cucudq.cn

Go:   json.Marshal(obj)
来源：http://qiv.jinghuilouyu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jar.dashuyun.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xbv.bbcook.cn

[K02] JSON 字符串转对象
来源：http://ohk.mhx1999.top

Py:   json.loads(s)
来源：http://dgl.jinyuanbaomall.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jau.jinqigfzy.top

JS:   JSON.parse(s)
来源：http://ool.zhixingplan.top

TS:   JSON.parse(s)
来源：http://sda.zycfv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lox.fehbvm.com

Go:   json.Unmarshal(data, &v)
来源：http://jdr.dianchejie.cn

Ruby: JSON.parse(s)
来源：http://eyg.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jrw.jqgufenzy.top

[K03] JSON 美化输出（带缩进）
来源：http://jdz.daxiang520.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ivn.sweek.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aog.gotoacloud.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mpm.shzxlz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qjq.ydjk.org.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://isp.sysykeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ztu.fehbvm.com

Ruby: JSON.pretty_generate(obj)
来源：http://djg.shzxlz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fsb.meibo888.top

[K04] 读取 JSON 文件
来源：http://uer.quarkkingdee.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jfr.zdqjudy.top


<!-- 参考信息 -->