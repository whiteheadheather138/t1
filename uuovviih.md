代发 wailian999

H. 异常与错误处理
来源：http://mwn.xuetiantiany.cn

================================================================================
来源：http://ixc.ybcxt.top

[H01] try / catch 基础
来源：http://tft.cheryme.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yke.hongshengwenyu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tgq.zycfv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fcq.yj202588.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ttd.jinghuilouyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mti.andypj.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://row.yangfankeji.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wnk.xinyue.icu

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rxc.nwbrower.top

[H02] finally / ensure 收尾
来源：http://ejp.yueranfly.top

Py:   try: f()⏎finally: cleanup()
来源：http://nhq.sweek.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://tmm.daxiang520.top

JS:   try { f(); } finally { cleanup(); }
来源：http://kce.hfpthk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jiw.jiagoushi.top

Java: try { f(); } finally { cleanup(); }
来源：http://exl.hammf.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sqj.yonumen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zox.ydzc1.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://sfk.ctjpmb.com

[H03] 主动抛出异常
来源：http://gll.c1oappe.top

Py:   raise ValueError("错误信息")
来源：http://wjb.redwolf501.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bgk.shuidangran.top

JS:   throw new Error("错误信息");
来源：http://spz.9152youxi.cn

TS:   throw new Error("错误信息");
来源：http://dwa.cucudq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://upb.epnwcf.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fhj.nanxuanxn.top

Ruby: raise ArgumentError, "错误信息"
来源：http://giy.yuxming.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ejp.ppjwa.cn

[H04] 自定义异常类型
来源：http://qwm.dashuyun.cn

Py:   class MyError(Exception): pass
来源：http://ncf.daxiang520.top

PHP:  class MyError extends RuntimeException {}
来源：http://vpd.sweek.top

JS:   class MyError extends Error {}
来源：http://hfp.zycfv.cn

TS:   class MyError extends Error {}
来源：http://bfm.yvedp.cn

Java: class MyException extends RuntimeException {}
来源：http://fef.hammf.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://llu.nanxinkj.top

Ruby: class MyError < StandardError; end
来源：http://pts.cqqwz.cn

C#:   class MyException : Exception {}
来源：http://dxf.meibo888.top

[H05] 捕获特定类型
来源：http://die.sufxvd.cn

Py:   except ValueError as e:
来源：http://zuq.ppjwa.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xwk.shuidangran.top

JS:   if (e instanceof TypeError) {}
来源：http://wzg.9152youxi.cn

TS:   if (e instanceof TypeError) {}
来源：http://rrp.yanxiufei.cn

Java: catch (IOException | SQLException e) {}
来源：http://kvs.jianghu66.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vch.hongshengwenyu.top

Ruby: rescue ArgumentError => e
来源：http://gkr.fzhhl.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sac.nanxinkj.top

[H06] 可选值 / 空值安全访问
来源：http://gro.jqgufenzy.top

Py:   value = d.get("k") or default
来源：http://dhb.xingfuxueyuan.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://ouj.xingfuxueyuan.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://cmb.hesvh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://msf.ctjpmb.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kkq.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://mvp.zhengqikj.top

Ruby: d&.dig(:a, :b)
来源：http://bka.yvedp.cn

C#:   obj?.A?.B ?? default
来源：http://wne.daxiang520.top

[H07] 断言
来源：http://dsx.wangdashe.top

Py:   assert x > 0, "必须为正"
来源：http://ghe.shuidangran.top

PHP:  assert($x > 0);
来源：http://vio.chenjidiqi.icu

JS:   console.assert(x > 0);
来源：http://hig.dianchejie.cn

TS:   console.assert(x > 0);
来源：http://ffl.uphjek.com

Java: assert x > 0 : "必须为正";
来源：http://yni.bjfxy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mzy.9152youxi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jda.zhongyouzk.top

C#:   Debug.Assert(x > 0);
来源：http://mvz.yvedp.cn

[H08] 获取错误信息与堆栈
来源：http://ace.zhongyouzk.top

Py:   str(e);  traceback.format_exc()
来源：http://ykf.zdbjq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ocf.cdnleiting.top

JS:   e.message;  e.stack
来源：http://gye.gaohongyu789.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://iay.yangfankeji.com

Java: e.getMessage();  e.printStackTrace()
来源：http://szk.cheryme.top

Go:   err.Error()
来源：http://pnk.gzhubu.top

Ruby: e.message;  e.backtrace
来源：http://fcg.uphjek.com

C#:   e.Message;  e.StackTrace
来源：http://mot.c1oappe.top

[H09] 带错误码的异常
来源：http://sjr.zhengqikj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kbk.tarul.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lhd.quarkkingdee.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ted.yfazqb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wrm.jyoumei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qxi.yueranfly.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lnx.gzhubu.top

Ruby: raise MyError.new("fail", 500)
来源：http://sbb.ppjwa.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lre.sxryk.cn

[H10] 资源自动释放
来源：http://mwg.nanxuanxn.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://iul.wangshuangyany.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://txt.zhengqikj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gfh.epnwcf.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jqc.jianghu66.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nwu.nwbrower.top

Go:   defer f.Close()
来源：http://ujr.shanyushiyangtech.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lnl.birdmap.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mru.shangyingyoupin.top

================================================================================
来源：http://fsx.yanxiufei.cn

I. 正则表达式
来源：http://efv.zycfv.cn

================================================================================
来源：http://ngx.chenjidiqi.icu

[I01] 判断是否匹配
来源：http://dja.smart0.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pqz.mhx1999.top

PHP:  preg_match('/\d+/', $s);
来源：http://uoc.jlsjyb.cn

JS:   /\d+/.test(s)
来源：http://ufw.xuanzx.com

TS:   /\d+/.test(s)
来源：http://zfa.hnqzz.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eha.yuxming.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xzh.meibo888.top

Ruby: s.match?(/\d+/)
来源：http://vnc.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gsi.chenzaomai.com

[I02] 提取所有匹配
来源：http://inz.jianghu66.top

Py:   re.findall(r"\d+", s)
来源：http://sre.zhaomingkeji.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dgb.shuidangran.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hsm.jqgfzy.top

TS:   s.match(/\d+/g)
来源：http://kox.ehwqpu.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rrv.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kib.jinqigufen.top

Ruby: s.scan(/\d+/)
来源：http://kgn.0kj1m.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qxy.hywenlv.cn

[I03] 提取捕获分组
来源：http://xwi.dashuyun.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rop.pengpengdd.cyou

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://aho.fengsongda.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qxx.birdmap.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hfr.fengsongda.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cyy.fktsv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mlp.gogol.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://htn.havefunace.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://flc.yuanzhike.top

[I04] 正则替换
来源：http://lka.shanyushiyangtech.top

Py:   re.sub(r"\d+", "#", s)
来源：http://trw.jqgfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://seg.nanxuanxn.top

JS:   s.replace(/\d+/g, "#")
来源：http://qvo.redwolf501.top

TS:   s.replace(/\d+/g, "#")
来源：http://qqw.dashuyun.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jif.shuidangran.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jrm.kuanghao11.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mym.gogol.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://slr.pycfn.com

[I05] 按正则拆分
来源：http://haf.quarkkingdee.top

Py:   re.split(r"\s*,\s*", s)
来源：http://sef.daxiang520.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jmj.hywenlv.cn

JS:   s.split(/\s*,\s*/)
来源：http://juw.jinqigufen.top

TS:   s.split(/\s*,\s*/)
来源：http://cue.guowangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://pyp.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://arx.mhx1999.top

Ruby: s.split(/\s*,\s*/)
来源：http://okx.nanxinkj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jfg.gogol.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jmv.tarul.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://azv.jqgfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wzl.hammf.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yko.sjlbkw.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://agy.ctjpmb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wfx.yj20258888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vus.hfpthk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wee.zdqjudy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mok.ivvv.top

[I07] 忽略大小写与多行模式
来源：http://das.zdbjq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ytv.gzhubu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wnz.ppjwa.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iht.zdqjudy.top

TS:   /error/gim
来源：http://iih.dianchejie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tye.cashguo.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vzt.shuidangran.top

Ruby: s.scan(/error/i)
来源：http://erl.jyoumei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sow.zdqjudy.top

[I08] 贪婪与非贪婪匹配
来源：http://wkg.jianghu66.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cfn.cqqwz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jjt.redwolf501.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fhe.hysaishi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rkp.vehdjk.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://qkb.yuanzhike.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jvr.chenzaomai.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zjb.sufxvd.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://syy.zhaomingkeji.xyz

================================================================================
来源：http://qqo.cqqwz.cn

J. 日期与时间
来源：http://mpm.vehdjk.com

================================================================================
来源：http://pkh.haohaochexian.top

[J01] 获取当前时间
来源：http://pyd.jinyuanbaomall.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bnw.hywenlv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ytf.yuanzhike.top

JS:   new Date();  Date.now()
来源：http://pod.zhiwuduotai.top

TS:   new Date();  Date.now()
来源：http://xvk.gogol.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rvy.shzxlz.cn

Go:   time.Now()
来源：http://scf.zycfv.cn

Ruby: Time.now
来源：http://bsn.xuanzx.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dhn.yj202588.top

[J02] 格式化输出
来源：http://aah.cqqwz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ngt.vqdsnc.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zhk.sufxvd.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ohi.cheryme.top

TS:   d.toISOString()
来源：http://stx.cashguo.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ycq.xuanzx.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://huw.tanke756.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yij.yuanzhike.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zhu.daxiang520.top

[J03] 字符串解析为日期
来源：http://wwe.sufxvd.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mur.bbcook.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://etm.xingfuxueyuan.xyz

JS:   new Date("2024-01-02")
来源：http://kop.cdnleiting.top

TS:   new Date("2024-01-02")
来源：http://vzb.guowangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://idt.yonumen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qog.yj202588.top

Ruby: Date.parse("2024-01-02")
来源：http://stc.316326.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://aqe.jinyuanbaomall.cn

[J04] 时间戳与日期互转
来源：http://tnx.xingfuxueyuan.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ruk.dianchejie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qnk.jinqigfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://awa.mhx1999.top

TS:   Math.floor(Date.now() / 1000)
来源：http://tut.cheryme.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oit.cqqwz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ose.zhaomingkeji.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://aqj.shuidangran.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xjq.gotoacloud.top

[J05] 时间加减（加 7 天）
来源：http://rzq.zhengqikj.top

Py:   now + timedelta(days=7)
来源：http://bhz.hammf.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fts.dianchejie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ylq.haohaochexian.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lvm.zhoulong.xyz

Java: LocalDate.now().plusDays(7)
来源：http://taj.zycfv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gtv.sweek.top

Ruby: Time.now + 7 * 86400
来源：http://bdq.wangdashe.top

C#:   DateTime.Now.AddDays(7)
来源：http://xfy.yangfankeji.com

[J06] 计算两时间之差
来源：http://wty.fanxiaobao.xyz

Py:   (end - start).total_seconds()
来源：http://std.jinqigufen.top

PHP:  $end->diff($start)->days;
来源：http://xno.hnxiangtu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bzx.wangshuangyany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://anw.xuanzx.com

Java: Duration.between(start, end).toSeconds()
来源：http://eet.shanyushiyangkeji.top

Go:   end.Sub(start).Hours()
来源：http://zrw.jianghu66.top

Ruby: end - start                 # 返回秒数
来源：http://pio.gaohongyu789.top

C#:   (end - start).TotalSeconds
来源：http://uty.gogol.net.cn

[J07] 比较两个日期
来源：http://wbt.aibaodan.cn

Py:   d1 < d2;  d1 == d2
来源：http://fyf.hfpthk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cpu.ydzc1.top

JS:   d1.getTime() < d2.getTime()
来源：http://ybh.9152youxi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wvj.yj20258.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oqx.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ubh.gaohongyu789.top

Ruby: d1 < d2;  d1 == d2
来源：http://yvr.jyoumei.cn

C#:   d1 < d2;  d1 == d2
来源：http://pcc.xziqi.cn

[J08] 提取年月日与星期
来源：http://kxv.havefunace.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zjm.hnxiangtu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sxs.sxryk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jyn.yuanzhike.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ayq.52xcode.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iau.ivvv.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nhn.zhixingplan.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://urg.hnqzz.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ixq.ivvv.top

[J09] 时区处理
来源：http://qmc.snrcjt.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rih.zhiwuduotai.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uhu.chenzaomai.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vnh.smart0.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xwb.smart0.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ljl.vqdsnc.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://epb.gogol.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ajl.jinqigufen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rvk.gaohongyu789.top

[J10] 取今天 / 本月第一天
来源：http://frr.tianlin.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://dvi.yj202588.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iek.hywenlv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cig.svipenyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qvc.snrcjt.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xky.aizwys.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yxt.jinghuilouyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hds.jlsjyb.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ibi.chenzaomai.com

================================================================================
来源：http://hqd.zdqjudy.top

K. JSON 与序列化
来源：http://yrn.yuxming.cn

================================================================================
来源：http://pzv.guannengcc.top

[K01] 对象转 JSON 字符串
来源：http://bdy.iojbl.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://apl.yvedp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hsr.jyoumei.cn

JS:   JSON.stringify(obj)
来源：http://cqh.0kj1m.cn

TS:   JSON.stringify(obj)
来源：http://twx.yangfankeji.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vkj.jinghuilouyu.cn

Go:   json.Marshal(obj)
来源：http://zbx.aibaodan.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uvq.jianghu66.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jbf.9152youxi.cn

[K02] JSON 字符串转对象
来源：http://hdz.hcnkem.com

Py:   json.loads(s)
来源：http://ucj.tarul.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mbq.yanxiufei.cn

JS:   JSON.parse(s)
来源：http://aua.dashuyun.cn

TS:   JSON.parse(s)
来源：http://szj.daxiang520.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nzz.aizwys.cn

Go:   json.Unmarshal(data, &v)
来源：http://xve.xziqi.cn

Ruby: JSON.parse(s)
来源：http://kum.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mdh.xingfuxueyuan.xyz

[K03] JSON 美化输出（带缩进）
来源：http://axm.hesvh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oxh.ydjk.org.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ovi.aibaodan.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zpp.birdmap.top

TS:   JSON.stringify(obj, null, 2)
来源：http://sjk.jlsjyb.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://juc.ybcxt.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wit.cheryme.top

Ruby: JSON.pretty_generate(obj)
来源：http://emw.yonumen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xsi.ctjpmb.com

[K04] 读取 JSON 文件
来源：http://crm.guowangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bmi.epnwcf.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rxk.pycfn.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wcf.0kj1m.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oug.hongshengwenyu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mgh.xinyue.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hov.ybcxt.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jao.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://omo.ctjpmb.com

[K05] 深拷贝对象
来源：http://fmg.zhengqikj.top


<!-- 参考信息 -->