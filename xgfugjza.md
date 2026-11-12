代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://boy.aibaodan.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://esu.yvedp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hli.zhoulong.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sry.nanxuanxn.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zna.fengsongda.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ouc.nanxinkj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wwq.xuetiantiany.cn

[H02] finally / ensure 收尾
来源：http://bps.iojbl.cn

Py:   try: f()⏎finally: cleanup()
来源：http://awn.gaohongyu789.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mbr.bbcook.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cvc.guowangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://lvn.jlsjyb.cn

Java: try { f(); } finally { cleanup(); }
来源：http://otc.hongshengwenyu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://utf.shangyingyoupin.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lgz.smart0.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://ulq.gaohongyu789.top

[H03] 主动抛出异常
来源：http://esz.chenjidiqi.icu

Py:   raise ValueError("错误信息")
来源：http://qie.zhongyouzk.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vcd.cheryme.top

JS:   throw new Error("错误信息");
来源：http://dxz.fktsv.cn

TS:   throw new Error("错误信息");
来源：http://qxf.nanxinkj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rfv.jqgfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hnf.pengpengdd.cyou

Ruby: raise ArgumentError, "错误信息"
来源：http://mjc.wangshuangyany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vwn.yuxming.cn

[H04] 自定义异常类型
来源：http://wnk.9152youxi.cn

Py:   class MyError(Exception): pass
来源：http://ulo.nanxinkj.top

PHP:  class MyError extends RuntimeException {}
来源：http://las.hongshengwenyu.top

JS:   class MyError extends Error {}
来源：http://ctf.epnwcf.com

TS:   class MyError extends Error {}
来源：http://chk.yonumen.top

Java: class MyException extends RuntimeException {}
来源：http://opn.jinqigfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uef.andypj.xyz

Ruby: class MyError < StandardError; end
来源：http://isw.zhiwuduotai.top

C#:   class MyException : Exception {}
来源：http://hoe.zhixingplan.top

[H05] 捕获特定类型
来源：http://zbo.epnwcf.com

Py:   except ValueError as e:
来源：http://huy.fengsongda.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ftu.shanyushiyangtech.top

JS:   if (e instanceof TypeError) {}
来源：http://wkc.cqqwz.cn

TS:   if (e instanceof TypeError) {}
来源：http://cwe.52xcode.cn

Java: catch (IOException | SQLException e) {}
来源：http://mpq.mhx1999.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vzu.ybcxt.top

Ruby: rescue ArgumentError => e
来源：http://qwu.sysykeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uto.c1oappe.top

[H06] 可选值 / 空值安全访问
来源：http://hoc.tianlin.xyz

Py:   value = d.get("k") or default
来源：http://hof.shangyingyoupin.top

PHP:  $v = $d["k"] ?? null;
来源：http://ezl.tanke756.top

JS:   obj?.a?.b;  d ?? default
来源：http://blr.havefunace.top

TS:   obj?.a?.b;  d ?? default
来源：http://iho.yj20258888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://txw.jqgfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wrj.yueranfly.top

Ruby: d&.dig(:a, :b)
来源：http://cdp.sufxvd.cn

C#:   obj?.A?.B ?? default
来源：http://pon.yj20258888.top

[H07] 断言
来源：http://vvo.snrcjt.cn

Py:   assert x > 0, "必须为正"
来源：http://yds.kuanghao11.cn

PHP:  assert($x > 0);
来源：http://fbv.jinqigfzy.top

JS:   console.assert(x > 0);
来源：http://ahj.shuidangran.top

TS:   console.assert(x > 0);
来源：http://iru.jinqigfzy.top

Java: assert x > 0 : "必须为正";
来源：http://pyi.wangdashe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://doz.tian-w.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lfs.hnqzz.top

C#:   Debug.Assert(x > 0);
来源：http://iyk.fktsv.cn

[H08] 获取错误信息与堆栈
来源：http://roi.jqgfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://yro.sysykeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vnt.havefunace.top

JS:   e.message;  e.stack
来源：http://ljy.feifeiyinyue.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qst.yongpay.top

Java: e.getMessage();  e.printStackTrace()
来源：http://svz.c1oappe.top

Go:   err.Error()
来源：http://heb.mhx1999.top

Ruby: e.message;  e.backtrace
来源：http://ifq.vehdjk.com

C#:   e.Message;  e.StackTrace
来源：http://ffq.guowangkeji.top

[H09] 带错误码的异常
来源：http://bgg.meibo888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lyy.zycfv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mem.mhx1999.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rmb.zdqjudy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kcy.ydzc1.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vjz.aizwys.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uvl.quarkkingdee.top

Ruby: raise MyError.new("fail", 500)
来源：http://nrf.yueranfly.top

C#:   // 自定义异常类中加 Code 属性
来源：http://iii.vehdjk.com

[H10] 资源自动释放
来源：http://ogq.smart0.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://mur.xuanzx.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dqn.hesvh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ydt.fehbvm.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://max.sweek.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lzk.smart0.xyz

Go:   defer f.Close()
来源：http://jnv.hammf.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hdj.fehbvm.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ood.yangfankeji.com

================================================================================
来源：http://rty.xinyue.icu

I. 正则表达式
来源：http://qof.yangfankeji.com

================================================================================
来源：http://ikz.snrcjt.cn

[I01] 判断是否匹配
来源：http://hqd.wangshuangyany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wbr.chenlongwang.top

PHP:  preg_match('/\d+/', $s);
来源：http://fuc.nanxuanxn.top

JS:   /\d+/.test(s)
来源：http://tir.jlsjyb.cn

TS:   /\d+/.test(s)
来源：http://gll.chenlongwang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fgk.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wji.yj20258.top

Ruby: s.match?(/\d+/)
来源：http://rbs.sjlbkw.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jep.ctjpmb.com

[I02] 提取所有匹配
来源：http://bkf.pycfn.com

Py:   re.findall(r"\d+", s)
来源：http://tsj.jinqigufen.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xzc.yuanzhike.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jak.zhijiandao.cn

TS:   s.match(/\d+/g)
来源：http://soj.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fqj.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qnr.yj202588.top

Ruby: s.scan(/\d+/)
来源：http://vhv.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nes.fanxiaobao.xyz

[I03] 提取捕获分组
来源：http://iar.shuidangran.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hnp.hnxiangtu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lct.tianlin.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hwb.ivvv.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gfk.haohaochexian.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jsn.zycfv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ews.zhixingplan.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mrg.jinqigufen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kfh.daria6918.cn

[I04] 正则替换
来源：http://eoh.jianghu66.top

Py:   re.sub(r"\d+", "#", s)
来源：http://aac.andypj.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iws.guannengcc.top

JS:   s.replace(/\d+/g, "#")
来源：http://ztr.ywan-chungtsiang.top

TS:   s.replace(/\d+/g, "#")
来源：http://rkr.fengsongda.top

Java: s.replaceAll("\\d+", "#")
来源：http://jpj.wangshuangyany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fiw.shzxlz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://als.quarkkingdee.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hlo.haohaochexian.top

[I05] 按正则拆分
来源：http://quf.xingfuxueyuan.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://nlx.ppjwa.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nlr.ppjwa.cn

JS:   s.split(/\s*,\s*/)
来源：http://oab.tarul.cn

TS:   s.split(/\s*,\s*/)
来源：http://mwc.yongpay.top

Java: s.split("\\s*,\\s*")
来源：http://xlz.jinghuilouyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wzv.birdmap.top

Ruby: s.split(/\s*,\s*/)
来源：http://rkw.daria6918.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rex.zhiwuduotai.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lqw.gzhubu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tfq.cqqwz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://drn.nwbrower.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://syq.jinyuanbaomall.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xkv.gogol.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vzz.xuetiantiany.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hww.ppjwa.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pzh.birdmap.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xak.uphjek.com

[I07] 忽略大小写与多行模式
来源：http://fdd.ybcxt.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ddm.sjlbkw.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uol.yonumen.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ugs.jinyuanbaomall.cn

TS:   /error/gim
来源：http://sep.fehbvm.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://aha.cdnleiting.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bzi.fanxiaobao.xyz

Ruby: s.scan(/error/i)
来源：http://ynl.svipenyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tft.zdbjq.cn

[I08] 贪婪与非贪婪匹配
来源：http://lhn.fzhhl.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pqj.zhaomingkeji.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ihr.zhoulong.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fhg.ywan-chungtsiang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://acy.bjfxy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://tyx.ybcxt.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nkc.hongshengwenyu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wfy.yuxming.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uzd.jinyuanbaomall.cn

================================================================================
来源：http://avt.havefunace.top

J. 日期与时间
来源：http://gxu.hnxiangtu.top

================================================================================
来源：http://zus.aizwys.cn

[J01] 获取当前时间
来源：http://vat.bbcook.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mmi.yuxming.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gsz.guowangkeji.top

JS:   new Date();  Date.now()
来源：http://jlv.andypj.xyz

TS:   new Date();  Date.now()
来源：http://azb.hywenlv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zts.jinqigufen.top

Go:   time.Now()
来源：http://ddk.yonumen.top

Ruby: Time.now
来源：http://hpg.fanxiaobao.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dzp.sjlbkw.cn

[J02] 格式化输出
来源：http://wsz.epnwcf.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ani.zdbjq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ynj.cucudq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kzt.hnqzz.top

TS:   d.toISOString()
来源：http://fxm.daria6918.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fdc.haohaochexian.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://caz.epnwcf.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qzo.shuidangran.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://paq.zhiwuduotai.top

[J03] 字符串解析为日期
来源：http://wkm.xuanzx.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sbc.shanyushiyangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zzm.uphjek.com

JS:   new Date("2024-01-02")
来源：http://zlo.feifeiyinyue.top

TS:   new Date("2024-01-02")
来源：http://rmi.sweek.top

Java: LocalDate.parse("2024-01-02")
来源：http://ior.zhixingplan.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fpl.gogol.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://nsb.ydjk.org.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wba.vqdsnc.cn

[J04] 时间戳与日期互转
来源：http://xgz.xuanzx.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oyc.fengsongda.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lxv.nanxuanxn.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rnm.jinyuanbaomall.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kun.zycfv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://atp.xinyue.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://btq.ydjk.org.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://emd.hongshengwenyu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dvg.yangfankeji.com

[J05] 时间加减（加 7 天）
来源：http://fxc.jinghuilouyu.cn

Py:   now + timedelta(days=7)
来源：http://tyx.kuanghao11.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dem.gaohongyu789.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jvu.aibaodan.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eti.bbcook.cn

Java: LocalDate.now().plusDays(7)
来源：http://dlr.tianlin.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://unl.jiagoushi.top

Ruby: Time.now + 7 * 86400
来源：http://nai.zdbjq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jve.shuidangran.top

[J06] 计算两时间之差
来源：http://cdj.haohaochexian.top

Py:   (end - start).total_seconds()
来源：http://zbl.fktsv.cn

PHP:  $end->diff($start)->days;
来源：http://ops.yuxming.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gim.fanxiaobao.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dtu.havefunace.top

Java: Duration.between(start, end).toSeconds()
来源：http://udk.zdqjudy.top

Go:   end.Sub(start).Hours()
来源：http://zlh.yfazqb.com

Ruby: end - start                 # 返回秒数
来源：http://szf.epnwcf.com

C#:   (end - start).TotalSeconds
来源：http://zna.cqqwz.cn

[J07] 比较两个日期
来源：http://tez.zhijiandao.cn

Py:   d1 < d2;  d1 == d2
来源：http://fwr.sjlbkw.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bmi.ivvv.top

JS:   d1.getTime() < d2.getTime()
来源：http://pja.andypj.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://umk.zdqjudy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://anv.chenlongwang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hys.birdmap.top

Ruby: d1 < d2;  d1 == d2
来源：http://uwd.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://zvw.xylfe.cn

[J08] 提取年月日与星期
来源：http://cdn.kuanghao11.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xee.hywenlv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lkl.fanxiaobao.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sjs.c1oappe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rdt.hfpthk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ybf.aizwys.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gfi.zycfv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uax.gogol.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dhp.yanxiufei.cn

[J09] 时区处理
来源：http://asd.0kj1m.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jvn.sweek.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tqk.zhongyouzk.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://frz.ydjk.org.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://skn.fehbvm.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rxz.yongpay.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ypc.aibaodan.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pdo.shanyushiyangtech.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lfr.shanyushiyangtech.top

[J10] 取今天 / 本月第一天
来源：http://fzj.xuanzx.com

Py:   date.today();  date.today().replace(day=1)
来源：http://ezx.zdqjudy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zmq.shangyingyoupin.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kmb.hysaishi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ren.cucudq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://asg.zhixingplan.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fyk.hcnkem.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uyu.bjfxy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wfc.gaohongyu789.top

================================================================================
来源：http://jub.cqqwz.cn

K. JSON 与序列化
来源：http://uaq.zdqjudy.top

================================================================================
来源：http://osu.smart0.xyz

[K01] 对象转 JSON 字符串
来源：http://cvx.chenzaomai.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kcp.jinghuilouyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vay.xziqi.cn

JS:   JSON.stringify(obj)
来源：http://zpk.ppjwa.cn

TS:   JSON.stringify(obj)
来源：http://bmq.dianchejie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zel.dashuyun.cn

Go:   json.Marshal(obj)
来源：http://nif.tanke756.top

Ruby: obj.to_json                                     // require "json"
来源：http://lvm.ydzc1.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xyu.hongshengwenyu.top

[K02] JSON 字符串转对象
来源：http://pza.jinyuanbaomall.cn

Py:   json.loads(s)
来源：http://nhs.cqqwz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://omt.gogol.net.cn

JS:   JSON.parse(s)
来源：http://ykm.shzxlz.cn

TS:   JSON.parse(s)
来源：http://wiz.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rrv.sxryk.cn

Go:   json.Unmarshal(data, &v)
来源：http://uut.tian-w.cn

Ruby: JSON.parse(s)
来源：http://jjp.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qaw.hysaishi.cn

[K03] JSON 美化输出（带缩进）
来源：http://mro.aizwys.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hbi.sxryk.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gpm.fehbvm.com

JS:   JSON.stringify(obj, null, 2)
来源：http://nit.birdmap.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ipe.hnqzz.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ehl.tanke756.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zlc.9152youxi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hsz.ehwqpu.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bkk.cqqwz.cn

[K04] 读取 JSON 文件
来源：http://lsc.shanyushiyangtech.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zti.shangyingyoupin.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bkb.zhixingplan.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wcz.vehdjk.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rsy.chenzaomai.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wic.shuidangran.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dbw.nanxuanxn.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cit.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qor.tian-w.cn

[K05] 深拷贝对象
来源：http://rdl.hammf.cn

Py:   copy.deepcopy(obj)
来源：http://klr.guannengcc.top

PHP:  unserialize(serialize($obj));
来源：http://bjj.hysaishi.cn

JS:   structuredClone(obj)
来源：http://fwz.daria6918.cn

TS:   structuredClone(obj)
来源：http://hzx.xuetiantiany.cn


<!-- 参考信息 -->