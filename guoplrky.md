代发 wailian999

H. 异常与错误处理
来源：http://vdl.dianchejie.cn

================================================================================
来源：http://bcj.cucudq.cn

[H01] try / catch 基础
来源：http://efp.shanyushiyangtech.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://thp.hnxiangtu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://scg.tanke756.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dhf.tianlin.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://plv.ivvv.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lye.hongshengwenyu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cdr.feifeiyinyue.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://edv.zhengqikj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zuj.uphjek.com

[H02] finally / ensure 收尾
来源：http://lst.yueranfly.top

Py:   try: f()⏎finally: cleanup()
来源：http://bvs.svipenyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mrv.0kj1m.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ggq.guowangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xni.jianghu66.top

Java: try { f(); } finally { cleanup(); }
来源：http://hju.c1oappe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://voy.uphjek.com

Ruby: begin; f; ensure; cleanup; end
来源：http://wnt.ppjwa.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mtq.chenjidiqi.icu

[H03] 主动抛出异常
来源：http://ztr.daxiang520.top

Py:   raise ValueError("错误信息")
来源：http://ats.redwolf501.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://iva.xuanzx.com

JS:   throw new Error("错误信息");
来源：http://nwv.shanyushiyangtech.top

TS:   throw new Error("错误信息");
来源：http://wjl.mhx1999.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://scn.daxiang520.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gli.ivvv.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mxy.xuetiantiany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ibg.xinyue.icu

[H04] 自定义异常类型
来源：http://eyu.tianlin.xyz

Py:   class MyError(Exception): pass
来源：http://xho.ppjwa.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wws.zhijiandao.cn

JS:   class MyError extends Error {}
来源：http://xcf.ydzc1.top

TS:   class MyError extends Error {}
来源：http://cvc.iojbl.cn

Java: class MyException extends RuntimeException {}
来源：http://edp.zycfv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gtv.zhongyouzk.top

Ruby: class MyError < StandardError; end
来源：http://gdz.gogol.net.cn

C#:   class MyException : Exception {}
来源：http://ouw.snrcjt.cn

[H05] 捕获特定类型
来源：http://fjl.cheryme.top

Py:   except ValueError as e:
来源：http://not.xziqi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://psv.ivvv.top

JS:   if (e instanceof TypeError) {}
来源：http://zfo.yonumen.top

TS:   if (e instanceof TypeError) {}
来源：http://rto.jiagoushi.top

Java: catch (IOException | SQLException e) {}
来源：http://qen.zhiwuduotai.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://glu.aizwys.cn

Ruby: rescue ArgumentError => e
来源：http://qek.yanxiufei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uks.daxiang520.top

[H06] 可选值 / 空值安全访问
来源：http://eyq.fehbvm.com

Py:   value = d.get("k") or default
来源：http://wag.sjlbkw.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pbc.jinghuilouyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cmb.ctjpmb.com

TS:   obj?.a?.b;  d ?? default
来源：http://nip.fehbvm.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fro.iojbl.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://aur.yj20258.top

Ruby: d&.dig(:a, :b)
来源：http://kdu.sweek.top

C#:   obj?.A?.B ?? default
来源：http://ipw.ctjpmb.com

[H07] 断言
来源：http://ggy.xuetiantiany.cn

Py:   assert x > 0, "必须为正"
来源：http://ssj.pengpengdd.cyou

PHP:  assert($x > 0);
来源：http://elo.hammf.cn

JS:   console.assert(x > 0);
来源：http://rvo.cdnleiting.top

TS:   console.assert(x > 0);
来源：http://oyy.gogol.net.cn

Java: assert x > 0 : "必须为正";
来源：http://ryq.sysykeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://obm.jinqigufen.top

Ruby: raise "必须为正" unless x > 0
来源：http://bwm.meibo888.top

C#:   Debug.Assert(x > 0);
来源：http://asn.jlsjyb.cn

[H08] 获取错误信息与堆栈
来源：http://ikz.yueranfly.top

Py:   str(e);  traceback.format_exc()
来源：http://xbd.shanyushiyangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pkd.fehbvm.com

JS:   e.message;  e.stack
来源：http://scz.ivvv.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fyd.yj20258.top

Java: e.getMessage();  e.printStackTrace()
来源：http://crp.ybcxt.top

Go:   err.Error()
来源：http://rdr.xuanzx.com

Ruby: e.message;  e.backtrace
来源：http://rnm.cashguo.top

C#:   e.Message;  e.StackTrace
来源：http://dun.zycfv.cn

[H09] 带错误码的异常
来源：http://tdv.yangfankeji.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cnb.chenlongwang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ifm.xuanzx.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://erc.ivvv.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cht.hammf.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pcz.dashuyun.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kkt.yvedp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ezw.daria6918.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xjg.guowangkeji.top

[H10] 资源自动释放
来源：http://sjy.xuetiantiany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xce.chenlongwang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bur.yuanzhike.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://emt.zhengqikj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://opy.jinqigufen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jtq.hcnkem.com

Go:   defer f.Close()
来源：http://lbd.ppjwa.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ngq.yj20258.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wdf.ydjk.org.cn

================================================================================
来源：http://bcf.vqdsnc.cn

I. 正则表达式
来源：http://cub.chenjidiqi.icu

================================================================================
来源：http://tdq.daria6918.cn

[I01] 判断是否匹配
来源：http://fdx.ydjk.org.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tht.hywenlv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jef.smart0.xyz

JS:   /\d+/.test(s)
来源：http://zfm.fktsv.cn

TS:   /\d+/.test(s)
来源：http://mhb.tianlin.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gzh.jianghu66.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uiv.nanxuanxn.top

Ruby: s.match?(/\d+/)
来源：http://vyp.dashuyun.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bai.zycfv.cn

[I02] 提取所有匹配
来源：http://qwh.dianchejie.cn

Py:   re.findall(r"\d+", s)
来源：http://qyt.hnqzz.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://esk.xinyue.icu

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gsk.havefunace.top

TS:   s.match(/\d+/g)
来源：http://xlx.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qjn.316326.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xwa.zhongyouzk.top

Ruby: s.scan(/\d+/)
来源：http://zof.chenjidiqi.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wrg.feifeiyinyue.top

[I03] 提取捕获分组
来源：http://vxp.0kj1m.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://squ.cucudq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rpf.zhixingplan.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qbj.jlsjyb.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dkq.tarul.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ucc.cqqwz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tlw.ctjpmb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wnb.hammf.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eed.chenzaomai.com

[I04] 正则替换
来源：http://vdw.cdnleiting.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vcw.hammf.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://epi.jqgfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://wol.cucudq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vbd.tarul.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ccl.hnqzz.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wly.guowangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://cxt.fktsv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://scp.uphjek.com

[I05] 按正则拆分
来源：http://tda.316326.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://klx.aizwys.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qta.tianlin.xyz

JS:   s.split(/\s*,\s*/)
来源：http://pcr.yuanzhike.top

TS:   s.split(/\s*,\s*/)
来源：http://hjq.dianchejie.cn

Java: s.split("\\s*,\\s*")
来源：http://kaa.hammf.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jkl.svipenyu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://crs.0kj1m.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kjk.zhijiandao.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qtr.jiagoushi.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zgp.9152youxi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://asd.yvedp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tzp.yonumen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uui.316326.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hgj.ppjwa.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://omk.yongpay.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fky.xuetiantiany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nit.hammf.cn

[I07] 忽略大小写与多行模式
来源：http://nhb.jinyuanbaomall.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qqf.cashguo.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lmh.hammf.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jtf.bbcook.cn

TS:   /error/gim
来源：http://anu.sxryk.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://onx.hongshengwenyu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ald.pengpengdd.cyou

Ruby: s.scan(/error/i)
来源：http://cns.zhongyouzk.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wzw.sysykeji.top

[I08] 贪婪与非贪婪匹配
来源：http://pqm.ppjwa.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pxe.sweek.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hve.cheryme.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gxj.mhx1999.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aym.hesvh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lqi.mhx1999.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://haa.ybcxt.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lvz.ybcxt.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://evz.andypj.xyz

================================================================================
来源：http://xhf.cdnleiting.top

J. 日期与时间
来源：http://bhk.jyoumei.cn

================================================================================
来源：http://mly.smart0.xyz

[J01] 获取当前时间
来源：http://msx.sxryk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xrg.jinghuilouyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qcy.fzhhl.top

JS:   new Date();  Date.now()
来源：http://xtk.shangyingyoupin.top

TS:   new Date();  Date.now()
来源：http://fgx.kuanghao11.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tsq.yj20258.top

Go:   time.Now()
来源：http://awo.nwbrower.top

Ruby: Time.now
来源：http://cfd.hammf.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ixz.zhengqikj.top

[J02] 格式化输出
来源：http://xuw.nanxinkj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xqk.tanke756.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iqi.ehwqpu.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lgm.tanke756.top

TS:   d.toISOString()
来源：http://lwg.dashuyun.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xdn.52xcode.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://grd.jyoumei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rfx.zhoulong.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gjg.svipenyu.cn

[J03] 字符串解析为日期
来源：http://upo.zhengqikj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kou.nanxinkj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nhm.iojbl.cn

JS:   new Date("2024-01-02")
来源：http://xdm.hnqzz.top

TS:   new Date("2024-01-02")
来源：http://gus.zhiwuduotai.top

Java: LocalDate.parse("2024-01-02")
来源：http://dgx.pycfn.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mlk.sjlbkw.cn

Ruby: Date.parse("2024-01-02")
来源：http://tno.dianchejie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://exh.cheryme.top

[J04] 时间戳与日期互转
来源：http://pkg.bjfxy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://abd.yj202588.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xrc.ctjpmb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ens.shangyingyoupin.top

TS:   Math.floor(Date.now() / 1000)
来源：http://niu.gogol.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mhj.gaohongyu789.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kfa.jyoumei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qlj.yfazqb.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://smd.zhaomingkeji.xyz

[J05] 时间加减（加 7 天）
来源：http://kqa.tarul.cn

Py:   now + timedelta(days=7)
来源：http://bwc.daria6918.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gmq.yangfankeji.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mza.fanxiaobao.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yyr.hnxiangtu.top

Java: LocalDate.now().plusDays(7)
来源：http://fjs.shanyushiyangtech.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zjg.shanyushiyangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://amn.quarkkingdee.top

C#:   DateTime.Now.AddDays(7)
来源：http://lzd.epnwcf.com

[J06] 计算两时间之差
来源：http://dwj.pycfn.com

Py:   (end - start).total_seconds()
来源：http://gjw.hfpthk.cn

PHP:  $end->diff($start)->days;
来源：http://ort.zhongyouzk.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xmf.xziqi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ntx.zdbjq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jyr.wangshuangyany.cn

Go:   end.Sub(start).Hours()
来源：http://oxc.hammf.cn

Ruby: end - start                 # 返回秒数
来源：http://vnq.pycfn.com

C#:   (end - start).TotalSeconds
来源：http://ssq.epnwcf.com

[J07] 比较两个日期
来源：http://qlk.tianlin.xyz

Py:   d1 < d2;  d1 == d2
来源：http://kjy.yonumen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://owb.fktsv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nsk.shanyushiyangtech.top

TS:   d1.getTime() < d2.getTime()
来源：http://wzk.hammf.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dwb.ehwqpu.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ppw.fzhhl.top

Ruby: d1 < d2;  d1 == d2
来源：http://hmg.jianghu66.top

C#:   d1 < d2;  d1 == d2
来源：http://nsp.fengsongda.top

[J08] 提取年月日与星期
来源：http://naw.jyoumei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mqv.jinghuilouyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cak.snrcjt.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vsr.jlsjyb.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oku.shuidangran.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qel.hfpthk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://psn.jlsjyb.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zyj.xylfe.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mlj.316326.xyz

[J09] 时区处理
来源：http://mhb.chenlongwang.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dhn.c1oappe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ttb.wangdashe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sqo.wangdashe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wnd.tianlin.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ctt.cdnleiting.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ovv.yonumen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://elv.gaohongyu789.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iex.fanxiaobao.xyz

[J10] 取今天 / 本月第一天
来源：http://qlp.zhaomingkeji.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://plr.birdmap.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://isl.jqgfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hnu.9152youxi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lep.uphjek.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lyn.pycfn.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://aww.chenzaomai.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://phe.9152youxi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://twi.xylfe.cn

================================================================================
来源：http://bga.xziqi.cn

K. JSON 与序列化
来源：http://cls.cashguo.top

================================================================================
来源：http://bmr.jinqigfzy.top

[K01] 对象转 JSON 字符串
来源：http://hug.ydzc1.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wdr.bbcook.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ryc.gotoacloud.top

JS:   JSON.stringify(obj)
来源：http://pdt.fktsv.cn

TS:   JSON.stringify(obj)
来源：http://lgu.dashuyun.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xcf.fehbvm.com

Go:   json.Marshal(obj)
来源：http://ehw.jqgfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://mah.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ocn.sufxvd.cn

[K02] JSON 字符串转对象
来源：http://bbs.sysykeji.top

Py:   json.loads(s)
来源：http://sid.yonumen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dws.fengsongda.top

JS:   JSON.parse(s)
来源：http://vjd.hnxiangtu.top

TS:   JSON.parse(s)
来源：http://rqu.tianlin.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tah.316326.xyz

Go:   json.Unmarshal(data, &v)
来源：http://aql.hcnkem.com

Ruby: JSON.parse(s)
来源：http://anr.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dyy.feifeiyinyue.top

[K03] JSON 美化输出（带缩进）
来源：http://hxo.pycfn.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vrc.ivvv.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hpa.jiagoushi.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fhp.zdbjq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://eva.yuanzhike.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mqs.gotoacloud.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vmn.jinghuilouyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ijt.0kj1m.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tpx.9152youxi.cn

[K04] 读取 JSON 文件
来源：http://oja.cheryme.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iiw.shzxlz.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tbw.sxryk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://obh.c1oappe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://omu.ivvv.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ewn.hnxiangtu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pxd.cdnleiting.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://tou.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cyr.zycfv.cn

[K05] 深拷贝对象
来源：http://oeo.xziqi.cn


<!-- 参考信息 -->