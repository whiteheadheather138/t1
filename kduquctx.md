代发 wailian999

H. 异常与错误处理
来源：http://szr.aizwys.cn

================================================================================
来源：http://hti.hammf.cn

[H01] try / catch 基础
来源：http://qic.gotoacloud.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zfb.xingfuxueyuan.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://myi.yuxming.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tzo.shuidangran.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vqk.9152youxi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://toz.hcnkem.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://haj.shanyushiyangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zfn.wangshuangyany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mti.yvedp.cn

[H02] finally / ensure 收尾
来源：http://piv.tianlin.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://ivt.cucudq.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qlx.feifeiyinyue.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wwc.sysykeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://khb.zhixingplan.top

Java: try { f(); } finally { cleanup(); }
来源：http://neo.zhaomingkeji.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://vdq.shanyushiyangtech.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vxb.sweek.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fnv.nanxinkj.top

[H03] 主动抛出异常
来源：http://zox.fengsongda.top

Py:   raise ValueError("错误信息")
来源：http://umi.bjfxy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wdc.yj20258.top

JS:   throw new Error("错误信息");
来源：http://jph.jiagoushi.top

TS:   throw new Error("错误信息");
来源：http://krw.jinqigufen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://crd.gotoacloud.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://afa.tarul.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zqa.haohaochexian.top

C#:   throw new ArgumentException("错误信息");
来源：http://gde.sxryk.cn

[H04] 自定义异常类型
来源：http://tec.cdnleiting.top

Py:   class MyError(Exception): pass
来源：http://eek.hywenlv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kwe.wangdashe.top

JS:   class MyError extends Error {}
来源：http://rnj.chenjidiqi.icu

TS:   class MyError extends Error {}
来源：http://dqg.haohaochexian.top

Java: class MyException extends RuntimeException {}
来源：http://lpz.gotoacloud.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lvz.epnwcf.com

Ruby: class MyError < StandardError; end
来源：http://olu.feifeiyinyue.top

C#:   class MyException : Exception {}
来源：http://pwk.cucudq.cn

[H05] 捕获特定类型
来源：http://erj.ydjk.org.cn

Py:   except ValueError as e:
来源：http://rwq.quarkkingdee.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rmg.dianchejie.cn

JS:   if (e instanceof TypeError) {}
来源：http://tee.tanke756.top

TS:   if (e instanceof TypeError) {}
来源：http://ben.bbcook.cn

Java: catch (IOException | SQLException e) {}
来源：http://oex.shzxlz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uzk.xinyue.icu

Ruby: rescue ArgumentError => e
来源：http://wtp.yueranfly.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rcc.kuanghao11.cn

[H06] 可选值 / 空值安全访问
来源：http://vnk.hammf.cn

Py:   value = d.get("k") or default
来源：http://jrq.tian-w.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bbt.gogol.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://keh.mhx1999.top

TS:   obj?.a?.b;  d ?? default
来源：http://mrj.jyoumei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rie.ivvv.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vtc.ydjk.org.cn

Ruby: d&.dig(:a, :b)
来源：http://nlb.jyoumei.cn

C#:   obj?.A?.B ?? default
来源：http://fzi.zycfv.cn

[H07] 断言
来源：http://egs.52xcode.cn

Py:   assert x > 0, "必须为正"
来源：http://pzz.ywan-chungtsiang.top

PHP:  assert($x > 0);
来源：http://hrb.bbcook.cn

JS:   console.assert(x > 0);
来源：http://rkz.aibaodan.cn

TS:   console.assert(x > 0);
来源：http://wig.pycfn.com

Java: assert x > 0 : "必须为正";
来源：http://gvi.bbcook.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yyn.pycfn.com

Ruby: raise "必须为正" unless x > 0
来源：http://mdw.dianchejie.cn

C#:   Debug.Assert(x > 0);
来源：http://vau.c1oappe.top

[H08] 获取错误信息与堆栈
来源：http://rxp.daxiang520.top

Py:   str(e);  traceback.format_exc()
来源：http://fmv.mhx1999.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rrt.cdnleiting.top

JS:   e.message;  e.stack
来源：http://yxt.yj20258.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://snu.havefunace.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jfr.ydzc1.top

Go:   err.Error()
来源：http://qpl.zhongyouzk.top

Ruby: e.message;  e.backtrace
来源：http://nxo.gaohongyu789.top

C#:   e.Message;  e.StackTrace
来源：http://ewd.jinghuilouyu.cn

[H09] 带错误码的异常
来源：http://tku.epnwcf.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wfo.xylfe.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cae.tianlin.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rxz.yangfankeji.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pzs.cucudq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rxs.cheryme.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zpp.hywenlv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gsr.fengsongda.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bwi.tarul.cn

[H10] 资源自动释放
来源：http://wke.yanxiufei.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://irp.daria6918.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://etr.redwolf501.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ujm.jqgfzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xau.cashguo.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ekh.bjfxy.top

Go:   defer f.Close()
来源：http://yea.hesvh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://chj.fzhhl.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xqp.feifeiyinyue.top

================================================================================
来源：http://geh.jiagoushi.top

I. 正则表达式
来源：http://cjw.birdmap.top

================================================================================
来源：http://iyt.ydjk.org.cn

[I01] 判断是否匹配
来源：http://buh.hysaishi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uex.zhijiandao.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dqj.ydjk.org.cn

JS:   /\d+/.test(s)
来源：http://vai.pengpengdd.cyou

TS:   /\d+/.test(s)
来源：http://bzv.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gmv.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://enc.zhiwuduotai.top

Ruby: s.match?(/\d+/)
来源：http://nzq.yonumen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wrn.xuanzx.com

[I02] 提取所有匹配
来源：http://tkx.xuanzx.com

Py:   re.findall(r"\d+", s)
来源：http://xxl.gotoacloud.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jpl.9152youxi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://emd.nanxuanxn.top

TS:   s.match(/\d+/g)
来源：http://xef.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://eye.mhx1999.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dwd.zhoulong.xyz

Ruby: s.scan(/\d+/)
来源：http://yrr.yuxming.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jls.shzxlz.cn

[I03] 提取捕获分组
来源：http://nda.jqgfzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xef.pycfn.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mbi.ydjk.org.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kqk.ybcxt.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cfe.c1oappe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fza.hnqzz.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aon.andypj.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://snv.gzhubu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sik.pycfn.com

[I04] 正则替换
来源：http://zqj.xuetiantiany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ofs.dashuyun.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qqp.9152youxi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://avy.tanke756.top

TS:   s.replace(/\d+/g, "#")
来源：http://wwv.jqgfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://onz.jianghu66.top

Go:   re.ReplaceAllString(s, "#")
来源：http://njk.hongshengwenyu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qea.hammf.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://aar.dianchejie.cn

[I05] 按正则拆分
来源：http://lnv.jlsjyb.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kwr.ydjk.org.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hsi.yueranfly.top

JS:   s.split(/\s*,\s*/)
来源：http://pvp.pengpengdd.cyou

TS:   s.split(/\s*,\s*/)
来源：http://ohr.wangdashe.top

Java: s.split("\\s*,\\s*")
来源：http://rxa.gzhubu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oax.ywan-chungtsiang.top

Ruby: s.split(/\s*,\s*/)
来源：http://yyi.jinqigfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nib.gaohongyu789.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ymm.nanxinkj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jwc.zhengqikj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tkr.hnxiangtu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ntx.tanke756.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://coy.fzhhl.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hhi.yj20258888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://def.shangyingyoupin.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://myh.zhijiandao.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jhg.bbcook.cn

[I07] 忽略大小写与多行模式
来源：http://ihl.birdmap.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fef.jinghuilouyu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dhy.sxryk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ggm.cucudq.cn

TS:   /error/gim
来源：http://gjr.ehwqpu.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jqc.yonumen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fjy.xinyue.icu

Ruby: s.scan(/error/i)
来源：http://efu.daxiang520.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ckx.fehbvm.com

[I08] 贪婪与非贪婪匹配
来源：http://qlr.zdqjudy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kuq.zycfv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bbr.fanxiaobao.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dpt.sweek.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hrh.snrcjt.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jqd.tian-w.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bbj.iojbl.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zdk.yj202588.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dbp.chenzaomai.com

================================================================================
来源：http://imn.chenjidiqi.icu

J. 日期与时间
来源：http://pib.bbcook.cn

================================================================================
来源：http://ocv.zdqjudy.top

[J01] 获取当前时间
来源：http://dhm.tanke756.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kce.yfazqb.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cxq.yanxiufei.cn

JS:   new Date();  Date.now()
来源：http://ftp.tian-w.cn

TS:   new Date();  Date.now()
来源：http://ykd.sweek.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yjk.ehwqpu.com

Go:   time.Now()
来源：http://haj.sufxvd.cn

Ruby: Time.now
来源：http://sug.guannengcc.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xcf.uphjek.com

[J02] 格式化输出
来源：http://dqm.zhijiandao.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kks.jinqigfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://enp.kuanghao11.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bjq.feifeiyinyue.top

TS:   d.toISOString()
来源：http://zth.ppjwa.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hmq.xinyue.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dcj.ctjpmb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eea.xuetiantiany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://owf.xinyue.icu

[J03] 字符串解析为日期
来源：http://woh.zhijiandao.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ufv.cdnleiting.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nky.shangyingyoupin.top

JS:   new Date("2024-01-02")
来源：http://hds.xylfe.cn

TS:   new Date("2024-01-02")
来源：http://rhn.cashguo.top

Java: LocalDate.parse("2024-01-02")
来源：http://bfz.c1oappe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://art.hfpthk.cn

Ruby: Date.parse("2024-01-02")
来源：http://ely.wangdashe.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://drh.ywan-chungtsiang.top

[J04] 时间戳与日期互转
来源：http://acl.tanke756.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yyg.tianlin.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nnt.gotoacloud.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xim.hywenlv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tso.ctjpmb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rhr.jinqigufen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://anj.c1oappe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lqp.ybcxt.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rma.smart0.xyz

[J05] 时间加减（加 7 天）
来源：http://jyv.dianchejie.cn

Py:   now + timedelta(days=7)
来源：http://hbo.ybcxt.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://yhn.ydzc1.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kdl.pycfn.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fau.fanxiaobao.xyz

Java: LocalDate.now().plusDays(7)
来源：http://ltu.yuxming.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://crr.birdmap.top

Ruby: Time.now + 7 * 86400
来源：http://eri.ivvv.top

C#:   DateTime.Now.AddDays(7)
来源：http://aaf.hfpthk.cn

[J06] 计算两时间之差
来源：http://xfz.yj20258.top

Py:   (end - start).total_seconds()
来源：http://bwh.bjfxy.top

PHP:  $end->diff($start)->days;
来源：http://oos.xinyue.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://isv.mhx1999.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gwh.daria6918.cn

Java: Duration.between(start, end).toSeconds()
来源：http://itj.dianchejie.cn

Go:   end.Sub(start).Hours()
来源：http://xpd.epnwcf.com

Ruby: end - start                 # 返回秒数
来源：http://kfr.jianghu66.top

C#:   (end - start).TotalSeconds
来源：http://cry.yangfankeji.com

[J07] 比较两个日期
来源：http://wee.yonumen.top

Py:   d1 < d2;  d1 == d2
来源：http://pon.vehdjk.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nwx.xuetiantiany.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rtd.9152youxi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://imm.xylfe.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kyh.xuetiantiany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xxh.zhijiandao.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qjx.jinqigfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://xam.nwbrower.top

[J08] 提取年月日与星期
来源：http://wss.zhixingplan.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://opu.kuanghao11.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hfy.xinyue.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vtz.fzhhl.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xxa.ivvv.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tmo.tarul.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://woz.hfpthk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lxe.guannengcc.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ypy.shzxlz.cn

[J09] 时区处理
来源：http://gvb.zhongyouzk.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bre.hcnkem.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dbz.yanxiufei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ckw.jinghuilouyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sxs.ydzc1.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://shy.52xcode.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://opd.fengsongda.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hzr.pengpengdd.cyou

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ocw.wangdashe.top

[J10] 取今天 / 本月第一天
来源：http://qep.sweek.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hmh.ctjpmb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pyt.yfazqb.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xhw.jinghuilouyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cbk.hcnkem.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://szd.tanke756.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://czp.zhengqikj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://scy.jyoumei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dtq.redwolf501.top

================================================================================
来源：http://rsw.yuxming.cn

K. JSON 与序列化
来源：http://elw.yvedp.cn

================================================================================
来源：http://xvb.0kj1m.cn

[K01] 对象转 JSON 字符串
来源：http://ypf.shuidangran.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gva.fehbvm.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tgs.cdnleiting.top

JS:   JSON.stringify(obj)
来源：http://koy.hfpthk.cn

TS:   JSON.stringify(obj)
来源：http://zih.xingfuxueyuan.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uxs.shanyushiyangkeji.top

Go:   json.Marshal(obj)
来源：http://lxr.yangfankeji.com

Ruby: obj.to_json                                     // require "json"
来源：http://mnt.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj)
来源：http://btx.ctjpmb.com

[K02] JSON 字符串转对象
来源：http://rej.tian-w.cn

Py:   json.loads(s)
来源：http://yxn.chenlongwang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vwi.xylfe.cn

JS:   JSON.parse(s)
来源：http://hvt.kuanghao11.cn

TS:   JSON.parse(s)
来源：http://vsd.tianlin.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zbx.xingfuxueyuan.xyz

Go:   json.Unmarshal(data, &v)
来源：http://ukf.xuanzx.com

Ruby: JSON.parse(s)
来源：http://mve.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gkv.shanyushiyangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://nkw.wangdashe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sya.uphjek.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ccj.fanxiaobao.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://lbc.bbcook.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://oct.kuanghao11.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ewi.sysykeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://emu.yongpay.top

Ruby: JSON.pretty_generate(obj)
来源：http://eql.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ssy.chenjidiqi.icu

[K04] 读取 JSON 文件
来源：http://sfk.sxryk.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zxl.birdmap.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://och.xinyue.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ndf.cheryme.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xwz.chenzaomai.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tfg.epnwcf.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://scf.xinyue.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://xoh.jinqigfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://icx.ctjpmb.com

[K05] 深拷贝对象
来源：http://tjn.ydzc1.top


<!-- 参考信息 -->