代发 wailian999

H. 异常与错误处理
来源：http://zuo.hnqzz.top

================================================================================
来源：http://sgc.sweek.top

[H01] try / catch 基础
来源：http://cry.hysaishi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vfd.svipenyu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://flk.jqgufenzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ebf.jinyuanbaomall.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cfh.pengpengdd.cyou

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ssr.shanyushiyangtech.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dyi.pycfn.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nuk.hesvh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tqc.gotoacloud.top

[H02] finally / ensure 收尾
来源：http://tsa.cashguo.top

Py:   try: f()⏎finally: cleanup()
来源：http://pwt.hesvh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sps.chenjidiqi.icu

JS:   try { f(); } finally { cleanup(); }
来源：http://dgc.redwolf501.top

TS:   try { f(); } finally { cleanup(); }
来源：http://obo.yvedp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jht.fktsv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hhi.nwbrower.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kvy.jinqigufen.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xhc.jinqigufen.top

[H03] 主动抛出异常
来源：http://qby.52xcode.cn

Py:   raise ValueError("错误信息")
来源：http://mzm.yueranfly.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xkc.52xcode.cn

JS:   throw new Error("错误信息");
来源：http://xry.pengpengdd.cyou

TS:   throw new Error("错误信息");
来源：http://kvo.mhx1999.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://tcn.daxiang520.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ffw.jlsjyb.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://poh.bjfxy.top

C#:   throw new ArgumentException("错误信息");
来源：http://eqn.zhiwuduotai.top

[H04] 自定义异常类型
来源：http://hig.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://itn.jlsjyb.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wtt.hammf.cn

JS:   class MyError extends Error {}
来源：http://lfh.dianchejie.cn

TS:   class MyError extends Error {}
来源：http://nbv.gotoacloud.top

Java: class MyException extends RuntimeException {}
来源：http://xap.zhiwuduotai.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xyb.xziqi.cn

Ruby: class MyError < StandardError; end
来源：http://evr.fanxiaobao.xyz

C#:   class MyException : Exception {}
来源：http://des.zhiwuduotai.top

[H05] 捕获特定类型
来源：http://alp.sysykeji.top

Py:   except ValueError as e:
来源：http://vvw.dashuyun.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ekf.haohaochexian.top

JS:   if (e instanceof TypeError) {}
来源：http://bgb.jiagoushi.top

TS:   if (e instanceof TypeError) {}
来源：http://gaq.jqgfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://dxt.9152youxi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tln.wangshuangyany.cn

Ruby: rescue ArgumentError => e
来源：http://cxt.zycfv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dqy.sweek.top

[H06] 可选值 / 空值安全访问
来源：http://dqy.cashguo.top

Py:   value = d.get("k") or default
来源：http://rnl.hammf.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vyz.svipenyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ikv.sufxvd.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zbu.cqqwz.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ptd.kuanghao11.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tbg.epnwcf.com

Ruby: d&.dig(:a, :b)
来源：http://bcf.aibaodan.cn

C#:   obj?.A?.B ?? default
来源：http://itt.wangdashe.top

[H07] 断言
来源：http://bkw.fktsv.cn

Py:   assert x > 0, "必须为正"
来源：http://lgk.c1oappe.top

PHP:  assert($x > 0);
来源：http://uec.yangfankeji.com

JS:   console.assert(x > 0);
来源：http://gld.zdbjq.cn

TS:   console.assert(x > 0);
来源：http://rrf.jinyuanbaomall.cn

Java: assert x > 0 : "必须为正";
来源：http://imm.kuanghao11.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://out.zhixingplan.top

Ruby: raise "必须为正" unless x > 0
来源：http://mnv.yangfankeji.com

C#:   Debug.Assert(x > 0);
来源：http://ata.mhx1999.top

[H08] 获取错误信息与堆栈
来源：http://xhy.jqgufenzy.top

Py:   str(e);  traceback.format_exc()
来源：http://qql.kuanghao11.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xur.yj202588.top

JS:   e.message;  e.stack
来源：http://iyj.jianghu66.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ygd.mhx1999.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bmr.xuanzx.com

Go:   err.Error()
来源：http://ztf.gaohongyu789.top

Ruby: e.message;  e.backtrace
来源：http://nky.ivvv.top

C#:   e.Message;  e.StackTrace
来源：http://uha.sxryk.cn

[H09] 带错误码的异常
来源：http://phd.dashuyun.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lmk.svipenyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rcq.jinqigfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jbk.zhiwuduotai.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://svu.feifeiyinyue.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eqc.shangyingyoupin.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dsy.nanxuanxn.top

Ruby: raise MyError.new("fail", 500)
来源：http://clb.feifeiyinyue.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gqc.chenzaomai.com

[H10] 资源自动释放
来源：http://moy.vehdjk.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://bhu.fanxiaobao.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hro.bjfxy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uhk.meibo888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bcw.fktsv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fsb.shzxlz.cn

Go:   defer f.Close()
来源：http://xnf.zhongyouzk.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hlj.zhijiandao.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vsf.cdnleiting.top

================================================================================
来源：http://tqi.cdnleiting.top

I. 正则表达式
来源：http://dyx.jinyuanbaomall.cn

================================================================================
来源：http://ylz.xinyue.icu

[I01] 判断是否匹配
来源：http://ygc.jinqigufen.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hbb.zhijiandao.cn

PHP:  preg_match('/\d+/', $s);
来源：http://svr.tanke756.top

JS:   /\d+/.test(s)
来源：http://xaf.chenlongwang.top

TS:   /\d+/.test(s)
来源：http://pop.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jja.yj20258.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zwa.andypj.xyz

Ruby: s.match?(/\d+/)
来源：http://xkg.9152youxi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bcb.ydzc1.top

[I02] 提取所有匹配
来源：http://oqv.dianchejie.cn

Py:   re.findall(r"\d+", s)
来源：http://soo.yj20258888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eqk.shangyingyoupin.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ytp.xingfuxueyuan.xyz

TS:   s.match(/\d+/g)
来源：http://hvx.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qyc.yuxming.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://orh.ywan-chungtsiang.top

Ruby: s.scan(/\d+/)
来源：http://kgb.mhx1999.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ksa.aibaodan.cn

[I03] 提取捕获分组
来源：http://vgo.gzhubu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://emm.jqgfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://frs.guowangkeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qmm.52xcode.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sfa.zhongyouzk.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jfz.wangdashe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ovs.cdnleiting.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qyo.hywenlv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dbu.tarul.cn

[I04] 正则替换
来源：http://mmr.shanyushiyangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://cpn.yvedp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://knp.sweek.top

JS:   s.replace(/\d+/g, "#")
来源：http://kzf.yueranfly.top

TS:   s.replace(/\d+/g, "#")
来源：http://kjx.jinyuanbaomall.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cci.smart0.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://ywx.shuidangran.top

Ruby: s.gsub(/\d+/, "#")
来源：http://buc.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ypr.jinqigufen.top

[I05] 按正则拆分
来源：http://rrg.feifeiyinyue.top

Py:   re.split(r"\s*,\s*", s)
来源：http://dxm.ydzc1.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mdx.yuanzhike.top

JS:   s.split(/\s*,\s*/)
来源：http://cvy.zhengqikj.top

TS:   s.split(/\s*,\s*/)
来源：http://tul.jlsjyb.cn

Java: s.split("\\s*,\\s*")
来源：http://dwm.nanxuanxn.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://skr.epnwcf.com

Ruby: s.split(/\s*,\s*/)
来源：http://mjw.shanyushiyangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yxp.vqdsnc.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nsv.havefunace.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rsm.0kj1m.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://src.zycfv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gdd.kuanghao11.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ekx.gzhubu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qca.gaohongyu789.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ayo.zhengqikj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vsw.zhengqikj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zzg.hnqzz.top

[I07] 忽略大小写与多行模式
来源：http://lrq.jinqigfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jqy.jinqigufen.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oea.aizwys.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bgu.tianlin.xyz

TS:   /error/gim
来源：http://myh.jqgfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://psk.9152youxi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sry.feifeiyinyue.top

Ruby: s.scan(/error/i)
来源：http://hia.fzhhl.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sci.xuanzx.com

[I08] 贪婪与非贪婪匹配
来源：http://qda.dianchejie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sny.nanxinkj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ich.cucudq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://epi.yangfankeji.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bqa.svipenyu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://doa.zhiwuduotai.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bbz.guowangkeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://klh.zdqjudy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uwv.shanyushiyangkeji.top

================================================================================
来源：http://ajo.yueranfly.top

J. 日期与时间
来源：http://zjq.zhaomingkeji.xyz

================================================================================
来源：http://ush.aizwys.cn

[J01] 获取当前时间
来源：http://jap.daxiang520.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ros.shanyushiyangtech.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ugh.zhengqikj.top

JS:   new Date();  Date.now()
来源：http://ohd.tarul.cn

TS:   new Date();  Date.now()
来源：http://pgx.bbcook.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kla.hfpthk.cn

Go:   time.Now()
来源：http://uod.aizwys.cn

Ruby: Time.now
来源：http://tpr.52xcode.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://eap.gzhubu.top

[J02] 格式化输出
来源：http://kid.tianlin.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jcv.jinqigufen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zim.zhongyouzk.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rmo.zhengqikj.top

TS:   d.toISOString()
来源：http://ntp.havefunace.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gqm.wangshuangyany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ybz.gotoacloud.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://afv.zhixingplan.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kbo.shanyushiyangkeji.top

[J03] 字符串解析为日期
来源：http://ili.shanyushiyangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qse.ybcxt.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vuh.ivvv.top

JS:   new Date("2024-01-02")
来源：http://szw.jiagoushi.top

TS:   new Date("2024-01-02")
来源：http://opf.gaohongyu789.top

Java: LocalDate.parse("2024-01-02")
来源：http://bgz.dianchejie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gjp.hysaishi.cn

Ruby: Date.parse("2024-01-02")
来源：http://oti.shuidangran.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nad.epnwcf.com

[J04] 时间戳与日期互转
来源：http://ima.mhx1999.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tnz.vehdjk.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yhp.sufxvd.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dbp.cheryme.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vht.xuanzx.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qdp.hongshengwenyu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zvk.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gxl.zhaomingkeji.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://aaf.bjfxy.top

[J05] 时间加减（加 7 天）
来源：http://yzb.sweek.top

Py:   now + timedelta(days=7)
来源：http://tuh.ehwqpu.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://xij.fehbvm.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bck.snrcjt.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kyi.ctjpmb.com

Java: LocalDate.now().plusDays(7)
来源：http://etz.gotoacloud.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ttn.wangdashe.top

Ruby: Time.now + 7 * 86400
来源：http://qah.quarkkingdee.top

C#:   DateTime.Now.AddDays(7)
来源：http://uzp.jqgfzy.top

[J06] 计算两时间之差
来源：http://jxn.guowangkeji.top

Py:   (end - start).total_seconds()
来源：http://xpd.cqqwz.cn

PHP:  $end->diff($start)->days;
来源：http://dgy.smart0.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nbo.yfazqb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sne.jinqigufen.top

Java: Duration.between(start, end).toSeconds()
来源：http://mmd.jyoumei.cn

Go:   end.Sub(start).Hours()
来源：http://jjj.andypj.xyz

Ruby: end - start                 # 返回秒数
来源：http://fcp.sweek.top

C#:   (end - start).TotalSeconds
来源：http://nbv.jiagoushi.top

[J07] 比较两个日期
来源：http://nst.nanxinkj.top

Py:   d1 < d2;  d1 == d2
来源：http://sxl.ydzc1.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vvw.jqgfzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://hkw.hywenlv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://oaa.jqgufenzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jbu.tarul.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://otq.ppjwa.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xex.cucudq.cn

C#:   d1 < d2;  d1 == d2
来源：http://rrx.ivvv.top

[J08] 提取年月日与星期
来源：http://geb.iojbl.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jjv.yuanzhike.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cug.kuanghao11.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kpy.haohaochexian.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tcf.hammf.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nxn.wangdashe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rdd.hnqzz.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wem.tarul.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://acw.zhaomingkeji.xyz

[J09] 时区处理
来源：http://gzz.yj202588.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://umy.xziqi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://djn.jinghuilouyu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://duo.gzhubu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://veq.tian-w.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vnl.xinyue.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mrn.shuidangran.top

Ruby: Time.now.getlocal("+08:00")
来源：http://cex.cqqwz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rcg.chenzaomai.com

[J10] 取今天 / 本月第一天
来源：http://pvq.yonumen.top

Py:   date.today();  date.today().replace(day=1)
来源：http://clq.uphjek.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vmf.shanyushiyangkeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vbw.yonumen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lmm.xinyue.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bhj.zhijiandao.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eyn.9152youxi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kex.xuetiantiany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zkh.yanxiufei.cn

================================================================================
来源：http://tno.0kj1m.cn

K. JSON 与序列化
来源：http://fhh.hcnkem.com

================================================================================
来源：http://gpn.mhx1999.top

[K01] 对象转 JSON 字符串
来源：http://vik.zhiwuduotai.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kuu.ybcxt.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dcs.chenjidiqi.icu

JS:   JSON.stringify(obj)
来源：http://qas.epnwcf.com

TS:   JSON.stringify(obj)
来源：http://zqp.zdbjq.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lhq.vehdjk.com

Go:   json.Marshal(obj)
来源：http://oyi.yvedp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://crm.nanxinkj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://pti.hnxiangtu.top

[K02] JSON 字符串转对象
来源：http://qdq.ydjk.org.cn

Py:   json.loads(s)
来源：http://pam.yvedp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gpf.jiagoushi.top

JS:   JSON.parse(s)
来源：http://qqb.hcnkem.com

TS:   JSON.parse(s)
来源：http://knq.hongshengwenyu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ahq.gzhubu.top

Go:   json.Unmarshal(data, &v)
来源：http://rzs.jinyuanbaomall.cn

Ruby: JSON.parse(s)
来源：http://ojz.jianghu66.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gjj.dashuyun.cn

[K03] JSON 美化输出（带缩进）
来源：http://zqn.fehbvm.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://alz.hfpthk.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ono.zdqjudy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://llt.fzhhl.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fep.hesvh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tno.zdqjudy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://paa.sufxvd.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mxi.hcnkem.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://enf.yongpay.top

[K04] 读取 JSON 文件
来源：http://kgo.gogol.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nva.redwolf501.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qvp.vqdsnc.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hql.aizwys.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zma.fktsv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vob.yuanzhike.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://spa.ydjk.org.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://uzg.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://psd.316326.xyz

[K05] 深拷贝对象
来源：http://sqo.zhongyouzk.top


<!-- 参考信息 -->