代发 wailian999

H. 异常与错误处理
来源：http://irh.c1oappe.top

================================================================================
来源：http://rbw.316326.xyz

[H01] try / catch 基础
来源：http://kgs.hnqzz.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cli.meibo888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pwp.yj20258.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mfd.hywenlv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://txw.zhoulong.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://erx.smart0.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ian.yj202588.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://koo.nanxinkj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ilr.gzhubu.top

[H02] finally / ensure 收尾
来源：http://oob.ctjpmb.com

Py:   try: f()⏎finally: cleanup()
来源：http://tle.yuanzhike.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://pxh.shuidangran.top

JS:   try { f(); } finally { cleanup(); }
来源：http://mrf.ydjk.org.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ubs.nanxinkj.top

Java: try { f(); } finally { cleanup(); }
来源：http://jdz.cucudq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rxt.guannengcc.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gsi.hywenlv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pmy.fehbvm.com

[H03] 主动抛出异常
来源：http://aay.yuxming.cn

Py:   raise ValueError("错误信息")
来源：http://vjz.zhengqikj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ess.bjfxy.top

JS:   throw new Error("错误信息");
来源：http://juy.snrcjt.cn

TS:   throw new Error("错误信息");
来源：http://zvp.zhongyouzk.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://urq.gogol.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mdo.birdmap.top

Ruby: raise ArgumentError, "错误信息"
来源：http://oqa.pengpengdd.cyou

C#:   throw new ArgumentException("错误信息");
来源：http://lhd.xuetiantiany.cn

[H04] 自定义异常类型
来源：http://trn.0kj1m.cn

Py:   class MyError(Exception): pass
来源：http://rsn.jiagoushi.top

PHP:  class MyError extends RuntimeException {}
来源：http://hky.jinghuilouyu.cn

JS:   class MyError extends Error {}
来源：http://dcg.ydjk.org.cn

TS:   class MyError extends Error {}
来源：http://fqe.fktsv.cn

Java: class MyException extends RuntimeException {}
来源：http://nsy.jinqigfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lkk.quarkkingdee.top

Ruby: class MyError < StandardError; end
来源：http://oxg.jinqigfzy.top

C#:   class MyException : Exception {}
来源：http://sta.zdbjq.cn

[H05] 捕获特定类型
来源：http://jqq.cashguo.top

Py:   except ValueError as e:
来源：http://wuu.yonumen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zwg.iojbl.cn

JS:   if (e instanceof TypeError) {}
来源：http://bbe.jinyuanbaomall.cn

TS:   if (e instanceof TypeError) {}
来源：http://aka.cashguo.top

Java: catch (IOException | SQLException e) {}
来源：http://fnd.kuanghao11.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ubl.zdbjq.cn

Ruby: rescue ArgumentError => e
来源：http://fxd.guannengcc.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uqq.andypj.xyz

[H06] 可选值 / 空值安全访问
来源：http://vkz.ctjpmb.com

Py:   value = d.get("k") or default
来源：http://mww.meibo888.top

PHP:  $v = $d["k"] ?? null;
来源：http://bfm.quarkkingdee.top

JS:   obj?.a?.b;  d ?? default
来源：http://zwi.52xcode.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rlz.guowangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jtc.sjlbkw.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fvd.hnxiangtu.top

Ruby: d&.dig(:a, :b)
来源：http://ifc.shangyingyoupin.top

C#:   obj?.A?.B ?? default
来源：http://jmi.jinqigfzy.top

[H07] 断言
来源：http://pwg.cheryme.top

Py:   assert x > 0, "必须为正"
来源：http://itc.ctjpmb.com

PHP:  assert($x > 0);
来源：http://gvq.snrcjt.cn

JS:   console.assert(x > 0);
来源：http://cbn.yj202588.top

TS:   console.assert(x > 0);
来源：http://vqp.birdmap.top

Java: assert x > 0 : "必须为正";
来源：http://rgk.sufxvd.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pgx.cheryme.top

Ruby: raise "必须为正" unless x > 0
来源：http://obw.fzhhl.top

C#:   Debug.Assert(x > 0);
来源：http://mwo.xuetiantiany.cn

[H08] 获取错误信息与堆栈
来源：http://gvz.snrcjt.cn

Py:   str(e);  traceback.format_exc()
来源：http://gra.guowangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ndl.zhixingplan.top

JS:   e.message;  e.stack
来源：http://sgb.yanxiufei.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zmk.aizwys.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jxk.ybcxt.top

Go:   err.Error()
来源：http://lwc.hywenlv.cn

Ruby: e.message;  e.backtrace
来源：http://bps.tian-w.cn

C#:   e.Message;  e.StackTrace
来源：http://pzg.chenjidiqi.icu

[H09] 带错误码的异常
来源：http://yhc.zhixingplan.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://roe.tanke756.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jpn.hammf.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aub.jlsjyb.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mjt.jianghu66.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tky.havefunace.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ose.feifeiyinyue.top

Ruby: raise MyError.new("fail", 500)
来源：http://sdq.tianlin.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://xto.chenjidiqi.icu

[H10] 资源自动释放
来源：http://fnt.jyoumei.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://agx.redwolf501.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yob.sufxvd.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://axi.nanxuanxn.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vba.0kj1m.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tcv.xuetiantiany.cn

Go:   defer f.Close()
来源：http://jdr.pycfn.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dsd.cqqwz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://goi.yvedp.cn

================================================================================
来源：http://yur.ybcxt.top

I. 正则表达式
来源：http://rgu.yanxiufei.cn

================================================================================
来源：http://tyd.hfpthk.cn

[I01] 判断是否匹配
来源：http://naw.cashguo.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rnq.quarkkingdee.top

PHP:  preg_match('/\d+/', $s);
来源：http://kaq.9152youxi.cn

JS:   /\d+/.test(s)
来源：http://kbu.shangyingyoupin.top

TS:   /\d+/.test(s)
来源：http://ljq.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pqk.ppjwa.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vlo.jianghu66.top

Ruby: s.match?(/\d+/)
来源：http://aeu.cheryme.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://riz.feifeiyinyue.top

[I02] 提取所有匹配
来源：http://tff.shanyushiyangtech.top

Py:   re.findall(r"\d+", s)
来源：http://zin.zhaomingkeji.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jyq.316326.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://for.zhiwuduotai.top

TS:   s.match(/\d+/g)
来源：http://cpv.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ieb.yj202588.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://upt.sxryk.cn

Ruby: s.scan(/\d+/)
来源：http://qou.epnwcf.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sxz.dashuyun.cn

[I03] 提取捕获分组
来源：http://whw.hywenlv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fpq.aibaodan.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://thx.chenlongwang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://don.jinyuanbaomall.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qiw.tarul.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ixh.fanxiaobao.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fjj.nanxuanxn.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qgm.xinyue.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ymg.ydzc1.top

[I04] 正则替换
来源：http://kka.dashuyun.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qlt.zhiwuduotai.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rpi.zdqjudy.top

JS:   s.replace(/\d+/g, "#")
来源：http://xjn.sjlbkw.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zge.daria6918.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zjo.xinyue.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://xly.tianlin.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://ovh.nanxinkj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fuz.svipenyu.cn

[I05] 按正则拆分
来源：http://bdj.ydjk.org.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://trs.epnwcf.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lwh.ppjwa.cn

JS:   s.split(/\s*,\s*/)
来源：http://xhw.meibo888.top

TS:   s.split(/\s*,\s*/)
来源：http://wss.hongshengwenyu.top

Java: s.split("\\s*,\\s*")
来源：http://job.xinyue.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xlb.hnxiangtu.top

Ruby: s.split(/\s*,\s*/)
来源：http://kbs.xuetiantiany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yog.xuetiantiany.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lmn.nanxinkj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://awe.aizwys.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dyn.vqdsnc.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oek.chenjidiqi.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rqi.nanxinkj.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hud.yj202588.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lhj.epnwcf.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ney.tianlin.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tnf.jinghuilouyu.cn

[I07] 忽略大小写与多行模式
来源：http://utv.cucudq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xea.guannengcc.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rvu.jinghuilouyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://czp.tianlin.xyz

TS:   /error/gim
来源：http://qmz.pycfn.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ifa.hesvh.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jmp.nwbrower.top

Ruby: s.scan(/error/i)
来源：http://rmo.yuxming.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bsm.guowangkeji.top

[I08] 贪婪与非贪婪匹配
来源：http://bpn.wangshuangyany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://twb.xinyue.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://izc.gzhubu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bev.chenlongwang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vjr.jqgufenzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://tnd.guowangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bmg.yongpay.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://shk.hammf.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nhj.zhengqikj.top

================================================================================
来源：http://zcd.cheryme.top

J. 日期与时间
来源：http://kiq.cqqwz.cn

================================================================================
来源：http://lzd.svipenyu.cn

[J01] 获取当前时间
来源：http://mqx.52xcode.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uje.ydjk.org.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ybp.meibo888.top

JS:   new Date();  Date.now()
来源：http://mpr.xuetiantiany.cn

TS:   new Date();  Date.now()
来源：http://mbk.gzhubu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dgh.vehdjk.com

Go:   time.Now()
来源：http://dnu.aibaodan.cn

Ruby: Time.now
来源：http://grj.yfazqb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zpv.havefunace.top

[J02] 格式化输出
来源：http://gjt.jinqigufen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uxn.fengsongda.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zed.tian-w.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rxp.jinyuanbaomall.cn

TS:   d.toISOString()
来源：http://qup.hesvh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sht.9152youxi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://twu.jlsjyb.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://btq.pycfn.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ejh.zdqjudy.top

[J03] 字符串解析为日期
来源：http://ush.ybcxt.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jyj.hcnkem.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sfx.316326.xyz

JS:   new Date("2024-01-02")
来源：http://vpe.yj20258.top

TS:   new Date("2024-01-02")
来源：http://nvq.shanyushiyangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://hbj.ydzc1.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vuq.dashuyun.cn

Ruby: Date.parse("2024-01-02")
来源：http://eje.yuxming.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tco.quarkkingdee.top

[J04] 时间戳与日期互转
来源：http://yks.birdmap.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mad.dashuyun.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://veg.tianlin.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://emj.tian-w.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://upc.zycfv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vdu.jqgufenzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nex.guannengcc.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://flu.wangshuangyany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nwd.zhaomingkeji.xyz

[J05] 时间加减（加 7 天）
来源：http://bzh.zhaomingkeji.xyz

Py:   now + timedelta(days=7)
来源：http://fuv.uphjek.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://vsz.jinqigfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://eej.jinqigufen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lcv.zdqjudy.top

Java: LocalDate.now().plusDays(7)
来源：http://tjl.redwolf501.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xxk.meibo888.top

Ruby: Time.now + 7 * 86400
来源：http://qbi.gogol.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://eom.zdbjq.cn

[J06] 计算两时间之差
来源：http://tfs.hywenlv.cn

Py:   (end - start).total_seconds()
来源：http://qvb.quarkkingdee.top

PHP:  $end->diff($start)->days;
来源：http://jjd.yongpay.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eza.jinqigufen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mhc.tanke756.top

Java: Duration.between(start, end).toSeconds()
来源：http://ocs.jinqigufen.top

Go:   end.Sub(start).Hours()
来源：http://wzy.sxryk.cn

Ruby: end - start                 # 返回秒数
来源：http://cqv.pycfn.com

C#:   (end - start).TotalSeconds
来源：http://mzm.zdqjudy.top

[J07] 比较两个日期
来源：http://xye.shanyushiyangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://vjp.jinqigufen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kgn.yanxiufei.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gkq.c1oappe.top

TS:   d1.getTime() < d2.getTime()
来源：http://fji.jinyuanbaomall.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rke.ybcxt.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://plx.xinyue.icu

Ruby: d1 < d2;  d1 == d2
来源：http://mjy.dashuyun.cn

C#:   d1 < d2;  d1 == d2
来源：http://geu.yongpay.top

[J08] 提取年月日与星期
来源：http://vkr.gotoacloud.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uaq.ywan-chungtsiang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dwr.hongshengwenyu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mnh.pycfn.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sun.cheryme.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tar.ybcxt.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pgr.andypj.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zok.ehwqpu.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bmb.yj20258.top

[J09] 时区处理
来源：http://opc.sxryk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jpv.gogol.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rfo.hcnkem.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ujr.smart0.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xng.vehdjk.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qzt.yuanzhike.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://euh.epnwcf.com

Ruby: Time.now.getlocal("+08:00")
来源：http://jnv.ywan-chungtsiang.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ttu.bjfxy.top

[J10] 取今天 / 本月第一天
来源：http://iwo.sjlbkw.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zck.hongshengwenyu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lhd.pycfn.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://liu.fanxiaobao.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://idq.zdqjudy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ydi.jqgufenzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nsv.zdbjq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yey.daxiang520.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yaq.dianchejie.cn

================================================================================
来源：http://gqi.316326.xyz

K. JSON 与序列化
来源：http://yjx.hcnkem.com

================================================================================
来源：http://cfk.zhijiandao.cn

[K01] 对象转 JSON 字符串
来源：http://fbx.yj20258888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tbn.hnqzz.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mjt.hywenlv.cn

JS:   JSON.stringify(obj)
来源：http://meq.hnqzz.top

TS:   JSON.stringify(obj)
来源：http://qth.birdmap.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jsz.bjfxy.top

Go:   json.Marshal(obj)
来源：http://llr.yj20258888.top

Ruby: obj.to_json                                     // require "json"
来源：http://pjq.316326.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://qme.cdnleiting.top

[K02] JSON 字符串转对象
来源：http://hoo.nanxinkj.top

Py:   json.loads(s)
来源：http://sei.cdnleiting.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jrw.cdnleiting.top

JS:   JSON.parse(s)
来源：http://zbo.jqgfzy.top

TS:   JSON.parse(s)
来源：http://mfd.shzxlz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tik.tian-w.cn

Go:   json.Unmarshal(data, &v)
来源：http://lqt.yuanzhike.top

Ruby: JSON.parse(s)
来源：http://oee.jianghu66.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vdc.yfazqb.com

[K03] JSON 美化输出（带缩进）
来源：http://str.shanyushiyangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nkm.zhongyouzk.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jff.wangdashe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mml.zhaomingkeji.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://tfp.andypj.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rrg.tanke756.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ajp.zhongyouzk.top

Ruby: JSON.pretty_generate(obj)
来源：http://egp.daxiang520.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jzx.dashuyun.cn

[K04] 读取 JSON 文件
来源：http://asv.zhongyouzk.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lto.daria6918.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qrz.zhoulong.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://csi.fktsv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dsk.jinqigfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hga.316326.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ahg.daria6918.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vlm.jianghu66.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zsd.shzxlz.cn

[K05] 深拷贝对象
来源：http://rgc.zdbjq.cn


<!-- 参考信息 -->