代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oxb.tanke756.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mdg.sjlbkw.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mau.zhiwuduotai.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xxi.zhongyouzk.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://msd.yvedp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wqu.hcnkem.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xsm.iojbl.cn

[H02] finally / ensure 收尾
来源：http://ldd.wangshuangyany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kmq.chenzaomai.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://jge.xinyue.icu

JS:   try { f(); } finally { cleanup(); }
来源：http://fto.sjlbkw.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://izt.yj20258888.top

Java: try { f(); } finally { cleanup(); }
来源：http://apo.jyoumei.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gok.gzhubu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://erq.dianchejie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jea.zhixingplan.top

[H03] 主动抛出异常
来源：http://cto.zdqjudy.top

Py:   raise ValueError("错误信息")
来源：http://grm.sweek.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rtt.xingfuxueyuan.xyz

JS:   throw new Error("错误信息");
来源：http://ygn.pycfn.com

TS:   throw new Error("错误信息");
来源：http://ozq.fzhhl.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mtq.vehdjk.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ero.chenlongwang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ash.shzxlz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://iir.nanxuanxn.top

[H04] 自定义异常类型
来源：http://itn.hesvh.cn

Py:   class MyError(Exception): pass
来源：http://sos.tian-w.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zmr.316326.xyz

JS:   class MyError extends Error {}
来源：http://ojh.yongpay.top

TS:   class MyError extends Error {}
来源：http://qez.tianlin.xyz

Java: class MyException extends RuntimeException {}
来源：http://fiu.zhongyouzk.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sdo.ehwqpu.com

Ruby: class MyError < StandardError; end
来源：http://dqm.redwolf501.top

C#:   class MyException : Exception {}
来源：http://imo.xuetiantiany.cn

[H05] 捕获特定类型
来源：http://xfr.cucudq.cn

Py:   except ValueError as e:
来源：http://beq.xingfuxueyuan.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://acn.ivvv.top

JS:   if (e instanceof TypeError) {}
来源：http://cza.xuanzx.com

TS:   if (e instanceof TypeError) {}
来源：http://ydc.tarul.cn

Java: catch (IOException | SQLException e) {}
来源：http://yox.jqgufenzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fdi.feifeiyinyue.top

Ruby: rescue ArgumentError => e
来源：http://ppl.yuxming.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vzc.pengpengdd.cyou

[H06] 可选值 / 空值安全访问
来源：http://dkq.sjlbkw.cn

Py:   value = d.get("k") or default
来源：http://xzd.tianlin.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://qvz.ydjk.org.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jeo.feifeiyinyue.top

TS:   obj?.a?.b;  d ?? default
来源：http://jxc.hesvh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bfs.hnxiangtu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hzt.cdnleiting.top

Ruby: d&.dig(:a, :b)
来源：http://anl.pycfn.com

C#:   obj?.A?.B ?? default
来源：http://esn.hysaishi.cn

[H07] 断言
来源：http://xfm.hammf.cn

Py:   assert x > 0, "必须为正"
来源：http://mfp.cqqwz.cn

PHP:  assert($x > 0);
来源：http://ati.yj20258888.top

JS:   console.assert(x > 0);
来源：http://jmu.sweek.top

TS:   console.assert(x > 0);
来源：http://skq.birdmap.top

Java: assert x > 0 : "必须为正";
来源：http://nbi.hesvh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dlh.9152youxi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://chh.svipenyu.cn

C#:   Debug.Assert(x > 0);
来源：http://qyj.yueranfly.top

[H08] 获取错误信息与堆栈
来源：http://sft.sjlbkw.cn

Py:   str(e);  traceback.format_exc()
来源：http://tyw.yuxming.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zte.0kj1m.cn

JS:   e.message;  e.stack
来源：http://ybs.sxryk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ahu.hfpthk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cbt.jlsjyb.cn

Go:   err.Error()
来源：http://mrz.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://wqc.guannengcc.top

C#:   e.Message;  e.StackTrace
来源：http://uuo.daxiang520.top

[H09] 带错误码的异常
来源：http://cdw.jiagoushi.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xqn.316326.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://ptz.meibo888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nen.shuidangran.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dvz.quarkkingdee.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vav.mhx1999.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mpf.cheryme.top

Ruby: raise MyError.new("fail", 500)
来源：http://nxc.jyoumei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ghh.shangyingyoupin.top

[H10] 资源自动释放
来源：http://coc.jqgfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mds.gzhubu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gbw.cdnleiting.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cay.jinghuilouyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wie.shzxlz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xck.redwolf501.top

Go:   defer f.Close()
来源：http://jzp.pengpengdd.cyou

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gkv.chenjidiqi.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fds.yj20258888.top

================================================================================
来源：http://jzd.shuidangran.top

I. 正则表达式
来源：http://zvd.fktsv.cn

================================================================================
来源：http://qwl.zhongyouzk.top

[I01] 判断是否匹配
来源：http://atm.smart0.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://brx.hesvh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qcz.hongshengwenyu.top

JS:   /\d+/.test(s)
来源：http://crm.0kj1m.cn

TS:   /\d+/.test(s)
来源：http://rgn.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gpf.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://obo.tian-w.cn

Ruby: s.match?(/\d+/)
来源：http://nwk.meibo888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ejv.ybcxt.top

[I02] 提取所有匹配
来源：http://imb.svipenyu.cn

Py:   re.findall(r"\d+", s)
来源：http://eik.bbcook.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mtv.yongpay.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://itf.ctjpmb.com

TS:   s.match(/\d+/g)
来源：http://cgx.jqgfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zab.guowangkeji.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://eit.fehbvm.com

Ruby: s.scan(/\d+/)
来源：http://iay.sjlbkw.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xjt.jinyuanbaomall.cn

[I03] 提取捕获分组
来源：http://wbp.chenzaomai.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wwd.ehwqpu.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nrp.yanxiufei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hus.jinqigfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pfd.yonumen.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uwx.hongshengwenyu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yhl.gaohongyu789.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iho.zhiwuduotai.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aov.shanyushiyangtech.top

[I04] 正则替换
来源：http://fzy.dashuyun.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nuu.ppjwa.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eke.yuxming.cn

JS:   s.replace(/\d+/g, "#")
来源：http://izm.zhixingplan.top

TS:   s.replace(/\d+/g, "#")
来源：http://qcg.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://mil.hysaishi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ivt.hywenlv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://thw.c1oappe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qvo.iojbl.cn

[I05] 按正则拆分
来源：http://xwl.ppjwa.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://iqh.yuanzhike.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://usy.ybcxt.top

JS:   s.split(/\s*,\s*/)
来源：http://mjb.chenlongwang.top

TS:   s.split(/\s*,\s*/)
来源：http://ago.tianlin.xyz

Java: s.split("\\s*,\\s*")
来源：http://jat.hammf.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ygb.redwolf501.top

Ruby: s.split(/\s*,\s*/)
来源：http://nwe.52xcode.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ees.jinqigufen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bva.yj20258888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ury.havefunace.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ozx.daria6918.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rhv.yanxiufei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xsx.redwolf501.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pda.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qvs.zhengqikj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zqf.gzhubu.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fma.sysykeji.top

[I07] 忽略大小写与多行模式
来源：http://fwh.yanxiufei.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rws.tian-w.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kka.cdnleiting.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mcg.bjfxy.top

TS:   /error/gim
来源：http://hdr.guannengcc.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://eam.hysaishi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ihm.jinyuanbaomall.cn

Ruby: s.scan(/error/i)
来源：http://rif.vqdsnc.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uga.hcnkem.com

[I08] 贪婪与非贪婪匹配
来源：http://jny.shangyingyoupin.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jkq.52xcode.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kgj.yj202588.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://feo.cucudq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lel.jqgufenzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rsz.zhaomingkeji.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zyv.xingfuxueyuan.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wpi.gaohongyu789.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://afu.316326.xyz

================================================================================
来源：http://mqk.xylfe.cn

J. 日期与时间
来源：http://pvm.yvedp.cn

================================================================================
来源：http://lwa.uphjek.com

[J01] 获取当前时间
来源：http://hzz.zhaomingkeji.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://cou.daria6918.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pwc.mhx1999.top

JS:   new Date();  Date.now()
来源：http://ruq.yuanzhike.top

TS:   new Date();  Date.now()
来源：http://rov.shuidangran.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dkv.feifeiyinyue.top

Go:   time.Now()
来源：http://tri.c1oappe.top

Ruby: Time.now
来源：http://fmd.gotoacloud.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zki.meibo888.top

[J02] 格式化输出
来源：http://uhm.snrcjt.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cld.guowangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xtd.fanxiaobao.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://acp.xuanzx.com

TS:   d.toISOString()
来源：http://bep.xuetiantiany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lcw.wangdashe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qow.zdbjq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lrk.smart0.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xeo.xingfuxueyuan.xyz

[J03] 字符串解析为日期
来源：http://gri.vqdsnc.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hlo.sufxvd.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gkv.gogol.net.cn

JS:   new Date("2024-01-02")
来源：http://nvu.jinqigufen.top

TS:   new Date("2024-01-02")
来源：http://iuk.yj20258.top

Java: LocalDate.parse("2024-01-02")
来源：http://duy.daria6918.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ipz.ehwqpu.com

Ruby: Date.parse("2024-01-02")
来源：http://xlu.zdbjq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://aqc.hesvh.cn

[J04] 时间戳与日期互转
来源：http://wzy.yj202588.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ebs.daria6918.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sqw.mhx1999.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pfo.xziqi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mej.ivvv.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jnq.daria6918.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yzb.hywenlv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hzf.aizwys.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://daf.shanyushiyangkeji.top

[J05] 时间加减（加 7 天）
来源：http://dpg.svipenyu.cn

Py:   now + timedelta(days=7)
来源：http://kqf.ydzc1.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ubm.chenzaomai.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bya.zhongyouzk.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pvv.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://qze.sjlbkw.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gqt.sweek.top

Ruby: Time.now + 7 * 86400
来源：http://exb.jqgfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://sop.hysaishi.cn

[J06] 计算两时间之差
来源：http://ncc.jlsjyb.cn

Py:   (end - start).total_seconds()
来源：http://irw.yuxming.cn

PHP:  $end->diff($start)->days;
来源：http://rat.zdqjudy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://siy.0kj1m.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vwu.chenzaomai.com

Java: Duration.between(start, end).toSeconds()
来源：http://yru.yueranfly.top

Go:   end.Sub(start).Hours()
来源：http://iuk.feifeiyinyue.top

Ruby: end - start                 # 返回秒数
来源：http://rqu.yj20258.top

C#:   (end - start).TotalSeconds
来源：http://tib.sufxvd.cn

[J07] 比较两个日期
来源：http://lzi.ydjk.org.cn

Py:   d1 < d2;  d1 == d2
来源：http://foz.9152youxi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uec.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://cdn.chenjidiqi.icu

TS:   d1.getTime() < d2.getTime()
来源：http://gtp.wangdashe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://avu.xziqi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bvm.ctjpmb.com

Ruby: d1 < d2;  d1 == d2
来源：http://jhk.gaohongyu789.top

C#:   d1 < d2;  d1 == d2
来源：http://jjm.cucudq.cn

[J08] 提取年月日与星期
来源：http://hhn.c1oappe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ikr.cdnleiting.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fsf.wangshuangyany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bdu.fzhhl.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sxg.pycfn.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rqx.gaohongyu789.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fmm.guowangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://daj.kuanghao11.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hxw.xuetiantiany.cn

[J09] 时区处理
来源：http://gch.kuanghao11.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fah.tanke756.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fht.yuanzhike.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nto.meibo888.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dlt.zhongyouzk.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dvc.ywan-chungtsiang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rgg.shzxlz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://eak.fktsv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://irq.jianghu66.top

[J10] 取今天 / 本月第一天
来源：http://yru.zhoulong.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://ssl.zhoulong.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jnt.tian-w.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hlf.ppjwa.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ymh.ydjk.org.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://srf.pengpengdd.cyou

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vyu.sxryk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qwd.shangyingyoupin.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yvf.haohaochexian.top

================================================================================
来源：http://sku.jinqigufen.top

K. JSON 与序列化
来源：http://lru.zhongyouzk.top

================================================================================
来源：http://wdb.fktsv.cn

[K01] 对象转 JSON 字符串
来源：http://pvi.hnqzz.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fhe.yonumen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nqo.shzxlz.cn

JS:   JSON.stringify(obj)
来源：http://sdn.feifeiyinyue.top

TS:   JSON.stringify(obj)
来源：http://shi.dianchejie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xec.zhixingplan.top

Go:   json.Marshal(obj)
来源：http://ida.fktsv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uvy.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://edp.fzhhl.top

[K02] JSON 字符串转对象
来源：http://ufy.yuanzhike.top

Py:   json.loads(s)
来源：http://lll.ywan-chungtsiang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://maj.jqgfzy.top

JS:   JSON.parse(s)
来源：http://rao.tianlin.xyz

TS:   JSON.parse(s)
来源：http://yef.zhongyouzk.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://evr.jinyuanbaomall.cn

Go:   json.Unmarshal(data, &v)
来源：http://xkf.zdbjq.cn

Ruby: JSON.parse(s)
来源：http://vas.hammf.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kiz.fktsv.cn

[K03] JSON 美化输出（带缩进）
来源：http://qqm.dianchejie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fki.sufxvd.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fbx.jinghuilouyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kxg.tarul.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://olg.jianghu66.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oxn.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bsa.hammf.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qbd.cdnleiting.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qoc.fanxiaobao.xyz

[K04] 读取 JSON 文件
来源：http://aas.zhixingplan.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sji.sjlbkw.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://piz.quarkkingdee.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sfr.ctjpmb.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://osj.gzhubu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mcd.iojbl.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://avj.cheryme.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://hkt.uphjek.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xot.wangdashe.top

[K05] 深拷贝对象
来源：http://tjv.tianlin.xyz

Py:   copy.deepcopy(obj)
来源：http://sig.gaohongyu789.top

PHP:  unserialize(serialize($obj));
来源：http://ueg.tanke756.top

JS:   structuredClone(obj)
来源：http://nlm.ywan-chungtsiang.top

TS:   structuredClone(obj)
来源：http://ose.gogol.net.cn


<!-- 参考信息 -->