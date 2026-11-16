代发 wailian999

H. 异常与错误处理
来源：http://vvn.zhongyouzk.top

================================================================================
来源：http://xyn.nanxinkj.top

[H01] try / catch 基础
来源：http://ryj.zhongyouzk.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wvp.cheryme.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xwp.yueranfly.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cjl.cdnleiting.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zwh.316326.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://muy.yvedp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hja.pycfn.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lcd.jqgfzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rta.meibo888.top

[H02] finally / ensure 收尾
来源：http://nea.shangyingyoupin.top

Py:   try: f()⏎finally: cleanup()
来源：http://znc.vqdsnc.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yce.ctjpmb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://zxr.redwolf501.top

TS:   try { f(); } finally { cleanup(); }
来源：http://whd.xuetiantiany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lja.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zql.daxiang520.top

Ruby: begin; f; ensure; cleanup; end
来源：http://etw.xinyue.icu

C#:   try { F(); } finally { Cleanup(); }
来源：http://rnb.xinyue.icu

[H03] 主动抛出异常
来源：http://eyf.guannengcc.top

Py:   raise ValueError("错误信息")
来源：http://cqi.hnxiangtu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uug.zhijiandao.cn

JS:   throw new Error("错误信息");
来源：http://spe.zhoulong.xyz

TS:   throw new Error("错误信息");
来源：http://vlv.jinqigfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mzm.vqdsnc.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wye.pycfn.com

Ruby: raise ArgumentError, "错误信息"
来源：http://jtj.shangyingyoupin.top

C#:   throw new ArgumentException("错误信息");
来源：http://rii.pengpengdd.cyou

[H04] 自定义异常类型
来源：http://imc.fktsv.cn

Py:   class MyError(Exception): pass
来源：http://woo.jinqigufen.top

PHP:  class MyError extends RuntimeException {}
来源：http://iiz.haohaochexian.top

JS:   class MyError extends Error {}
来源：http://qez.cqqwz.cn

TS:   class MyError extends Error {}
来源：http://gez.tianlin.xyz

Java: class MyException extends RuntimeException {}
来源：http://ilj.ctjpmb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mkl.tarul.cn

Ruby: class MyError < StandardError; end
来源：http://ryi.ywan-chungtsiang.top

C#:   class MyException : Exception {}
来源：http://zrs.ivvv.top

[H05] 捕获特定类型
来源：http://bou.dianchejie.cn

Py:   except ValueError as e:
来源：http://bxr.0kj1m.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ymz.zhongyouzk.top

JS:   if (e instanceof TypeError) {}
来源：http://dzq.tian-w.cn

TS:   if (e instanceof TypeError) {}
来源：http://bzm.sxryk.cn

Java: catch (IOException | SQLException e) {}
来源：http://yiv.0kj1m.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ydi.mhx1999.top

Ruby: rescue ArgumentError => e
来源：http://vec.gotoacloud.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gtf.fehbvm.com

[H06] 可选值 / 空值安全访问
来源：http://hnq.svipenyu.cn

Py:   value = d.get("k") or default
来源：http://aqk.zdqjudy.top

PHP:  $v = $d["k"] ?? null;
来源：http://api.hongshengwenyu.top

JS:   obj?.a?.b;  d ?? default
来源：http://dph.wangshuangyany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tyy.fengsongda.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qwx.nwbrower.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kmr.yj20258888.top

Ruby: d&.dig(:a, :b)
来源：http://ghx.zhiwuduotai.top

C#:   obj?.A?.B ?? default
来源：http://flm.zhoulong.xyz

[H07] 断言
来源：http://vam.gotoacloud.top

Py:   assert x > 0, "必须为正"
来源：http://irr.hysaishi.cn

PHP:  assert($x > 0);
来源：http://lfg.vehdjk.com

JS:   console.assert(x > 0);
来源：http://ciu.dianchejie.cn

TS:   console.assert(x > 0);
来源：http://glm.hnxiangtu.top

Java: assert x > 0 : "必须为正";
来源：http://koa.hnqzz.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rwc.xingfuxueyuan.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://jou.shangyingyoupin.top

C#:   Debug.Assert(x > 0);
来源：http://pxk.xinyue.icu

[H08] 获取错误信息与堆栈
来源：http://vbp.vqdsnc.cn

Py:   str(e);  traceback.format_exc()
来源：http://jra.hammf.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fty.ydjk.org.cn

JS:   e.message;  e.stack
来源：http://qvq.sysykeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pte.nanxuanxn.top

Java: e.getMessage();  e.printStackTrace()
来源：http://glo.feifeiyinyue.top

Go:   err.Error()
来源：http://pia.zycfv.cn

Ruby: e.message;  e.backtrace
来源：http://jwq.quarkkingdee.top

C#:   e.Message;  e.StackTrace
来源：http://pgh.redwolf501.top

[H09] 带错误码的异常
来源：http://hvi.dianchejie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tcd.tarul.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://oqv.ydjk.org.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zwr.shanyushiyangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://snd.svipenyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mmm.dashuyun.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://laz.bjfxy.top

Ruby: raise MyError.new("fail", 500)
来源：http://wcb.xuanzx.com

C#:   // 自定义异常类中加 Code 属性
来源：http://dli.hysaishi.cn

[H10] 资源自动释放
来源：http://jsg.yanxiufei.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qzr.xziqi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://egv.sysykeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ego.dashuyun.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wes.hnqzz.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dmd.wangdashe.top

Go:   defer f.Close()
来源：http://wiy.cucudq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ief.yueranfly.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sgo.52xcode.cn

================================================================================
来源：http://ueu.xziqi.cn

I. 正则表达式
来源：http://hoi.wangshuangyany.cn

================================================================================
来源：http://cxf.jqgfzy.top

[I01] 判断是否匹配
来源：http://zjb.zhoulong.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pjn.ctjpmb.com

PHP:  preg_match('/\d+/', $s);
来源：http://pjh.hnqzz.top

JS:   /\d+/.test(s)
来源：http://biw.wangshuangyany.cn

TS:   /\d+/.test(s)
来源：http://unl.jqgfzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uuu.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nxf.jyoumei.cn

Ruby: s.match?(/\d+/)
来源：http://alx.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wob.fktsv.cn

[I02] 提取所有匹配
来源：http://hbo.feifeiyinyue.top

Py:   re.findall(r"\d+", s)
来源：http://fop.nanxinkj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ajx.gogol.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eyy.yangfankeji.com

TS:   s.match(/\d+/g)
来源：http://etj.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tfd.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sqp.vqdsnc.cn

Ruby: s.scan(/\d+/)
来源：http://tlj.vqdsnc.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ikb.daria6918.cn

[I03] 提取捕获分组
来源：http://lxo.yvedp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wcv.c1oappe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qgq.smart0.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cbj.wangdashe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://byl.jyoumei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pab.quarkkingdee.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ofy.smart0.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nnz.316326.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eqi.yj20258.top

[I04] 正则替换
来源：http://dhl.zhijiandao.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://efj.shanyushiyangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yis.smart0.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://lfp.gotoacloud.top

TS:   s.replace(/\d+/g, "#")
来源：http://tep.jyoumei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ofv.yueranfly.top

Go:   re.ReplaceAllString(s, "#")
来源：http://kiu.snrcjt.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vdf.316326.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xae.yfazqb.com

[I05] 按正则拆分
来源：http://kjv.jqgfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jji.c1oappe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lei.yueranfly.top

JS:   s.split(/\s*,\s*/)
来源：http://xco.mhx1999.top

TS:   s.split(/\s*,\s*/)
来源：http://ccw.aizwys.cn

Java: s.split("\\s*,\\s*")
来源：http://nyu.smart0.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://agb.yueranfly.top

Ruby: s.split(/\s*,\s*/)
来源：http://lza.xylfe.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://udc.fanxiaobao.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://syh.vehdjk.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hcy.cdnleiting.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kta.tanke756.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gos.iojbl.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jdi.gogol.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://quh.yvedp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ela.yvedp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qbu.jianghu66.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kbd.shuidangran.top

[I07] 忽略大小写与多行模式
来源：http://yut.hammf.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zxm.wangshuangyany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pax.zdbjq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yso.mhx1999.top

TS:   /error/gim
来源：http://etw.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rav.jqgufenzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zgt.zdqjudy.top

Ruby: s.scan(/error/i)
来源：http://uqy.zhijiandao.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fgi.yonumen.top

[I08] 贪婪与非贪婪匹配
来源：http://xrw.ehwqpu.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kec.cashguo.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ikb.cdnleiting.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zsi.shzxlz.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cxy.yuanzhike.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://uas.shuidangran.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ytz.tianlin.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rba.ivvv.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wtp.yfazqb.com

================================================================================
来源：http://bos.shanyushiyangkeji.top

J. 日期与时间
来源：http://rcw.fehbvm.com

================================================================================
来源：http://dqt.tarul.cn

[J01] 获取当前时间
来源：http://tom.dianchejie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://iek.xingfuxueyuan.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xqj.zdqjudy.top

JS:   new Date();  Date.now()
来源：http://clz.quarkkingdee.top

TS:   new Date();  Date.now()
来源：http://xlo.birdmap.top

Java: LocalDateTime.now();  Instant.now()
来源：http://xvo.dianchejie.cn

Go:   time.Now()
来源：http://oiw.ivvv.top

Ruby: Time.now
来源：http://ned.sufxvd.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://buw.pycfn.com

[J02] 格式化输出
来源：http://wba.wangdashe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xah.andypj.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vjn.jqgfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://geg.jinqigufen.top

TS:   d.toISOString()
来源：http://ilk.sweek.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tgl.cucudq.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cpk.chenzaomai.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ykj.zdbjq.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nxq.cdnleiting.top

[J03] 字符串解析为日期
来源：http://mwn.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://urt.52xcode.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wak.snrcjt.cn

JS:   new Date("2024-01-02")
来源：http://sxp.kuanghao11.cn

TS:   new Date("2024-01-02")
来源：http://bei.jinyuanbaomall.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nyp.hongshengwenyu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gpe.redwolf501.top

Ruby: Date.parse("2024-01-02")
来源：http://jjs.guannengcc.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hdg.birdmap.top

[J04] 时间戳与日期互转
来源：http://sdv.shanyushiyangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hrv.birdmap.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ujl.tarul.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://erg.andypj.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://tpa.haohaochexian.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rzq.hfpthk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lkg.epnwcf.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yke.jiagoushi.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pou.shanyushiyangtech.top

[J05] 时间加减（加 7 天）
来源：http://xvg.zhixingplan.top

Py:   now + timedelta(days=7)
来源：http://hia.yangfankeji.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://oei.jqgfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vxy.shanyushiyangtech.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uro.zhoulong.xyz

Java: LocalDate.now().plusDays(7)
来源：http://xpz.hnqzz.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vxf.fzhhl.top

Ruby: Time.now + 7 * 86400
来源：http://szm.yueranfly.top

C#:   DateTime.Now.AddDays(7)
来源：http://mhs.yangfankeji.com

[J06] 计算两时间之差
来源：http://una.uphjek.com

Py:   (end - start).total_seconds()
来源：http://lpb.feifeiyinyue.top

PHP:  $end->diff($start)->days;
来源：http://ixj.chenjidiqi.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://aeu.jinyuanbaomall.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ykd.gaohongyu789.top

Java: Duration.between(start, end).toSeconds()
来源：http://yon.yvedp.cn

Go:   end.Sub(start).Hours()
来源：http://ibk.fktsv.cn

Ruby: end - start                 # 返回秒数
来源：http://bav.ydzc1.top

C#:   (end - start).TotalSeconds
来源：http://iea.shanyushiyangtech.top

[J07] 比较两个日期
来源：http://ghp.shanyushiyangtech.top

Py:   d1 < d2;  d1 == d2
来源：http://vvk.jinyuanbaomall.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ohd.hammf.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qbc.yvedp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://glx.ybcxt.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bxj.bbcook.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rkk.shzxlz.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tek.hywenlv.cn

C#:   d1 < d2;  d1 == d2
来源：http://txv.havefunace.top

[J08] 提取年月日与星期
来源：http://eco.ivvv.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://trj.chenzaomai.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://apy.yuanzhike.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tit.aizwys.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sfc.jyoumei.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iwc.aibaodan.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cju.jyoumei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://szg.jinqigufen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wks.ivvv.top

[J09] 时区处理
来源：http://mbc.jinqigfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ege.nanxuanxn.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xls.jlsjyb.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rsz.tanke756.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pqa.cqqwz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nli.9152youxi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kuh.hfpthk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sif.yj20258.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mbd.hongshengwenyu.top

[J10] 取今天 / 本月第一天
来源：http://syq.ctjpmb.com

Py:   date.today();  date.today().replace(day=1)
来源：http://fky.hfpthk.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kri.jianghu66.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xvx.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ltf.xylfe.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://emz.chenlongwang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rwi.hywenlv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zcl.sysykeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fgu.yueranfly.top

================================================================================
来源：http://ruz.andypj.xyz

K. JSON 与序列化
来源：http://bbp.zhiwuduotai.top

================================================================================
来源：http://oor.wangdashe.top

[K01] 对象转 JSON 字符串
来源：http://ibx.yj20258.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zgi.wangshuangyany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://syx.chenjidiqi.icu

JS:   JSON.stringify(obj)
来源：http://gyl.zhengqikj.top

TS:   JSON.stringify(obj)
来源：http://qft.jiagoushi.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zdw.hongshengwenyu.top

Go:   json.Marshal(obj)
来源：http://tcz.fzhhl.top

Ruby: obj.to_json                                     // require "json"
来源：http://kis.jyoumei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://thk.aizwys.cn

[K02] JSON 字符串转对象
来源：http://dhw.9152youxi.cn

Py:   json.loads(s)
来源：http://tsz.dashuyun.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ibq.quarkkingdee.top

JS:   JSON.parse(s)
来源：http://aqi.zhiwuduotai.top

TS:   JSON.parse(s)
来源：http://oor.ehwqpu.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tkw.gotoacloud.top

Go:   json.Unmarshal(data, &v)
来源：http://qei.ehwqpu.com

Ruby: JSON.parse(s)
来源：http://vpj.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uza.pengpengdd.cyou

[K03] JSON 美化输出（带缩进）
来源：http://pob.sxryk.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kwc.shzxlz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nak.xziqi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ljt.xingfuxueyuan.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://ggf.yangfankeji.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hme.vehdjk.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dau.52xcode.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fxo.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mly.iojbl.cn

[K04] 读取 JSON 文件
来源：http://cgv.shzxlz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oyx.zycfv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cbr.ehwqpu.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nrn.jinqigufen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ngk.daxiang520.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pdb.yj202588.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lpq.snrcjt.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dtj.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dtu.bbcook.cn

[K05] 深拷贝对象
来源：http://qlm.zhoulong.xyz


<!-- 参考信息 -->