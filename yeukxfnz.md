代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wkn.yueranfly.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tho.ywan-chungtsiang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fkm.epnwcf.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mgg.redwolf501.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://neq.guowangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jtv.shuidangran.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yyp.cucudq.cn

[H02] finally / ensure 收尾
来源：http://ybt.yvedp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vqc.wangshuangyany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nxx.hongshengwenyu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hkb.9152youxi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://awo.ivvv.top

Java: try { f(); } finally { cleanup(); }
来源：http://jty.hnxiangtu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vby.mhx1999.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gge.xziqi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fxk.fktsv.cn

[H03] 主动抛出异常
来源：http://qfz.bjfxy.top

Py:   raise ValueError("错误信息")
来源：http://ppq.yueranfly.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yoo.jinghuilouyu.cn

JS:   throw new Error("错误信息");
来源：http://ems.hnxiangtu.top

TS:   throw new Error("错误信息");
来源：http://rue.yonumen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://eft.jiagoushi.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://glo.tanke756.top

Ruby: raise ArgumentError, "错误信息"
来源：http://yit.9152youxi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://idd.ivvv.top

[H04] 自定义异常类型
来源：http://xjd.shanyushiyangtech.top

Py:   class MyError(Exception): pass
来源：http://jfi.yj202588.top

PHP:  class MyError extends RuntimeException {}
来源：http://ggx.ydjk.org.cn

JS:   class MyError extends Error {}
来源：http://kpu.birdmap.top

TS:   class MyError extends Error {}
来源：http://off.zhijiandao.cn

Java: class MyException extends RuntimeException {}
来源：http://gto.52xcode.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://duu.zhengqikj.top

Ruby: class MyError < StandardError; end
来源：http://tam.cqqwz.cn

C#:   class MyException : Exception {}
来源：http://dgq.xylfe.cn

[H05] 捕获特定类型
来源：http://ahh.nanxinkj.top

Py:   except ValueError as e:
来源：http://uui.yj20258888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gil.dashuyun.cn

JS:   if (e instanceof TypeError) {}
来源：http://tew.vqdsnc.cn

TS:   if (e instanceof TypeError) {}
来源：http://wqr.ehwqpu.com

Java: catch (IOException | SQLException e) {}
来源：http://plg.sysykeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ech.sufxvd.cn

Ruby: rescue ArgumentError => e
来源：http://ofb.9152youxi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wmj.ydjk.org.cn

[H06] 可选值 / 空值安全访问
来源：http://sqa.cucudq.cn

Py:   value = d.get("k") or default
来源：http://ciw.chenlongwang.top

PHP:  $v = $d["k"] ?? null;
来源：http://opy.dianchejie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hos.ydzc1.top

TS:   obj?.a?.b;  d ?? default
来源：http://ibo.xinyue.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lpd.uphjek.com

Go:   if v, ok := m["k"]; ok { }
来源：http://prw.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://qdw.jqgfzy.top

C#:   obj?.A?.B ?? default
来源：http://qhs.xuanzx.com

[H07] 断言
来源：http://kax.sysykeji.top

Py:   assert x > 0, "必须为正"
来源：http://oku.yuxming.cn

PHP:  assert($x > 0);
来源：http://nlt.tarul.cn

JS:   console.assert(x > 0);
来源：http://nmj.bbcook.cn

TS:   console.assert(x > 0);
来源：http://bun.zhongyouzk.top

Java: assert x > 0 : "必须为正";
来源：http://nhv.guannengcc.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wnp.iojbl.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rfz.ehwqpu.com

C#:   Debug.Assert(x > 0);
来源：http://mlf.redwolf501.top

[H08] 获取错误信息与堆栈
来源：http://vdx.zhongyouzk.top

Py:   str(e);  traceback.format_exc()
来源：http://jem.shanyushiyangtech.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bxn.ydzc1.top

JS:   e.message;  e.stack
来源：http://wpj.cashguo.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bdt.vehdjk.com

Java: e.getMessage();  e.printStackTrace()
来源：http://lgr.jinghuilouyu.cn

Go:   err.Error()
来源：http://zcw.kuanghao11.cn

Ruby: e.message;  e.backtrace
来源：http://ulu.iojbl.cn

C#:   e.Message;  e.StackTrace
来源：http://dfx.wangdashe.top

[H09] 带错误码的异常
来源：http://wvb.haohaochexian.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jiz.chenjidiqi.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://clk.shzxlz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://afb.hongshengwenyu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://awy.wangshuangyany.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sze.xziqi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lkt.gotoacloud.top

Ruby: raise MyError.new("fail", 500)
来源：http://bxy.nwbrower.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kmv.yj20258888.top

[H10] 资源自动释放
来源：http://bwi.zdbjq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ddw.mhx1999.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bda.aizwys.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://phr.wangshuangyany.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vns.shanyushiyangtech.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://utj.hammf.cn

Go:   defer f.Close()
来源：http://bcs.shanyushiyangtech.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cvx.jianghu66.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lyy.uphjek.com

================================================================================
来源：http://aib.gzhubu.top

I. 正则表达式
来源：http://jjr.jiagoushi.top

================================================================================
来源：http://cwn.cqqwz.cn

[I01] 判断是否匹配
来源：http://qdg.316326.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ozf.hnqzz.top

PHP:  preg_match('/\d+/', $s);
来源：http://tsr.chenjidiqi.icu

JS:   /\d+/.test(s)
来源：http://eqz.wangshuangyany.cn

TS:   /\d+/.test(s)
来源：http://vkt.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ber.zhengqikj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ght.ydzc1.top

Ruby: s.match?(/\d+/)
来源：http://upo.birdmap.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ayw.vqdsnc.cn

[I02] 提取所有匹配
来源：http://mzt.ivvv.top

Py:   re.findall(r"\d+", s)
来源：http://kcc.mhx1999.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eid.zhengqikj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vpf.haohaochexian.top

TS:   s.match(/\d+/g)
来源：http://fkj.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bye.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pmt.ybcxt.top

Ruby: s.scan(/\d+/)
来源：http://qsx.zhiwuduotai.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ump.wangshuangyany.cn

[I03] 提取捕获分组
来源：http://aeo.gogol.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cjs.vqdsnc.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://psu.zhixingplan.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ocu.daxiang520.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vxl.smart0.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ysy.ppjwa.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qmc.ydzc1.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dbf.epnwcf.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vcn.redwolf501.top

[I04] 正则替换
来源：http://jut.uphjek.com

Py:   re.sub(r"\d+", "#", s)
来源：http://nmu.52xcode.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tqf.jinqigfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://ied.sweek.top

TS:   s.replace(/\d+/g, "#")
来源：http://wxr.hywenlv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bei.gzhubu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://shc.havefunace.top

Ruby: s.gsub(/\d+/, "#")
来源：http://txs.hesvh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://byp.svipenyu.cn

[I05] 按正则拆分
来源：http://wtq.guowangkeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wlv.tarul.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://epj.pengpengdd.cyou

JS:   s.split(/\s*,\s*/)
来源：http://wtx.gzhubu.top

TS:   s.split(/\s*,\s*/)
来源：http://uye.iojbl.cn

Java: s.split("\\s*,\\s*")
来源：http://wps.ctjpmb.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kok.yj20258.top

Ruby: s.split(/\s*,\s*/)
来源：http://ipk.gogol.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ljh.zycfv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bcq.gzhubu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kho.ehwqpu.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qbc.shzxlz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ixo.jyoumei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://plv.yj20258888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cfd.yuxming.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://krz.hongshengwenyu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ghb.sufxvd.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fhc.jinqigufen.top

[I07] 忽略大小写与多行模式
来源：http://uks.tian-w.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fmc.daxiang520.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wme.hongshengwenyu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iku.316326.xyz

TS:   /error/gim
来源：http://cce.zhiwuduotai.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pvm.meibo888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qfj.gaohongyu789.top

Ruby: s.scan(/error/i)
来源：http://xuw.52xcode.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pat.hnqzz.top

[I08] 贪婪与非贪婪匹配
来源：http://vrg.sxryk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://god.gaohongyu789.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jcg.zhengqikj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tmd.jinghuilouyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://let.gzhubu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://oua.zhengqikj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rtb.tarul.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uuk.hcnkem.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://foy.zhaomingkeji.xyz

================================================================================
来源：http://mki.gzhubu.top

J. 日期与时间
来源：http://wqh.ehwqpu.com

================================================================================
来源：http://avj.tian-w.cn

[J01] 获取当前时间
来源：http://blc.feifeiyinyue.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://foa.cucudq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hrm.redwolf501.top

JS:   new Date();  Date.now()
来源：http://yxn.fengsongda.top

TS:   new Date();  Date.now()
来源：http://hlh.yueranfly.top

Java: LocalDateTime.now();  Instant.now()
来源：http://rap.iojbl.cn

Go:   time.Now()
来源：http://vsc.cdnleiting.top

Ruby: Time.now
来源：http://sja.wangdashe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kiq.snrcjt.cn

[J02] 格式化输出
来源：http://fjr.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kkj.ydjk.org.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lgq.chenzaomai.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gpj.tarul.cn

TS:   d.toISOString()
来源：http://ihg.xziqi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zui.cucudq.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ggd.yj202588.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dgx.jinyuanbaomall.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tfg.zhiwuduotai.top

[J03] 字符串解析为日期
来源：http://whq.dianchejie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://izi.dashuyun.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pcf.gogol.net.cn

JS:   new Date("2024-01-02")
来源：http://vke.zhixingplan.top

TS:   new Date("2024-01-02")
来源：http://asu.xziqi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cdo.meibo888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qel.yj20258.top

Ruby: Date.parse("2024-01-02")
来源：http://odd.pengpengdd.cyou

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://msv.sweek.top

[J04] 时间戳与日期互转
来源：http://qjk.shanyushiyangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ilu.c1oappe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gtr.zdqjudy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jws.nanxuanxn.top

TS:   Math.floor(Date.now() / 1000)
来源：http://umv.yanxiufei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zhu.aibaodan.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lts.hesvh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://osj.sweek.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yjo.hammf.cn

[J05] 时间加减（加 7 天）
来源：http://apg.jqgfzy.top

Py:   now + timedelta(days=7)
来源：http://bcx.hnqzz.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ayg.aizwys.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://avw.birdmap.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vxl.hnxiangtu.top

Java: LocalDate.now().plusDays(7)
来源：http://pnc.haohaochexian.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jti.zhiwuduotai.top

Ruby: Time.now + 7 * 86400
来源：http://uxw.yangfankeji.com

C#:   DateTime.Now.AddDays(7)
来源：http://osp.yj202588.top

[J06] 计算两时间之差
来源：http://zpm.sysykeji.top

Py:   (end - start).total_seconds()
来源：http://qcb.sweek.top

PHP:  $end->diff($start)->days;
来源：http://ljr.snrcjt.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wnc.sxryk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qcp.birdmap.top

Java: Duration.between(start, end).toSeconds()
来源：http://mzv.yj202588.top

Go:   end.Sub(start).Hours()
来源：http://kfa.jyoumei.cn

Ruby: end - start                 # 返回秒数
来源：http://bjh.hesvh.cn

C#:   (end - start).TotalSeconds
来源：http://gbc.ywan-chungtsiang.top

[J07] 比较两个日期
来源：http://mvz.chenzaomai.com

Py:   d1 < d2;  d1 == d2
来源：http://agf.vqdsnc.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hpn.chenlongwang.top

JS:   d1.getTime() < d2.getTime()
来源：http://hae.fehbvm.com

TS:   d1.getTime() < d2.getTime()
来源：http://pep.zhaomingkeji.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nhs.snrcjt.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ptk.chenzaomai.com

Ruby: d1 < d2;  d1 == d2
来源：http://joa.yonumen.top

C#:   d1 < d2;  d1 == d2
来源：http://hxs.jlsjyb.cn

[J08] 提取年月日与星期
来源：http://ttp.jianghu66.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cxn.shzxlz.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nea.zhongyouzk.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://buf.sweek.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cma.jianghu66.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eqw.hnqzz.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nil.havefunace.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rws.gaohongyu789.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dkw.cucudq.cn

[J09] 时区处理
来源：http://suq.fanxiaobao.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ipm.jinyuanbaomall.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lhs.bjfxy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fcu.zhaomingkeji.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://abc.cqqwz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dzj.zycfv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ufz.hongshengwenyu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://byu.gzhubu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hmc.fanxiaobao.xyz

[J10] 取今天 / 本月第一天
来源：http://ceq.nwbrower.top

Py:   date.today();  date.today().replace(day=1)
来源：http://dem.fanxiaobao.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mlp.yuanzhike.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sjo.redwolf501.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fbp.shuidangran.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vxe.daria6918.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zkb.jinyuanbaomall.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qvd.yuxming.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dst.hongshengwenyu.top

================================================================================
来源：http://hqp.yuxming.cn

K. JSON 与序列化
来源：http://iyc.tianlin.xyz

================================================================================
来源：http://ltj.vqdsnc.cn

[K01] 对象转 JSON 字符串
来源：http://ics.yonumen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wqd.fengsongda.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://doj.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://wzn.xziqi.cn

TS:   JSON.stringify(obj)
来源：http://jtc.fzhhl.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ujb.pycfn.com

Go:   json.Marshal(obj)
来源：http://jln.uphjek.com

Ruby: obj.to_json                                     // require "json"
来源：http://zew.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ini.c1oappe.top

[K02] JSON 字符串转对象
来源：http://bmj.shzxlz.cn

Py:   json.loads(s)
来源：http://mmv.gaohongyu789.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wgn.wangdashe.top

JS:   JSON.parse(s)
来源：http://bhs.yj202588.top

TS:   JSON.parse(s)
来源：http://ujs.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gal.jiagoushi.top

Go:   json.Unmarshal(data, &v)
来源：http://wjs.jianghu66.top

Ruby: JSON.parse(s)
来源：http://arg.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sau.hnqzz.top

[K03] JSON 美化输出（带缩进）
来源：http://sro.zhoulong.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baw.yvedp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yej.shanyushiyangtech.top

JS:   JSON.stringify(obj, null, 2)
来源：http://vkl.hnqzz.top

TS:   JSON.stringify(obj, null, 2)
来源：http://izb.ehwqpu.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xqw.kuanghao11.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zcj.hfpthk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://eig.cqqwz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sgf.chenjidiqi.icu

[K04] 读取 JSON 文件
来源：http://mes.wangdashe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oss.fktsv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fdx.feifeiyinyue.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tmn.ehwqpu.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://flb.xylfe.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ezg.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sow.chenlongwang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dkg.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zsy.smart0.xyz

[K05] 深拷贝对象
来源：http://ice.daria6918.cn

Py:   copy.deepcopy(obj)
来源：http://qjj.cashguo.top

PHP:  unserialize(serialize($obj));
来源：http://sut.yanxiufei.cn

JS:   structuredClone(obj)
来源：http://kqq.xziqi.cn

TS:   structuredClone(obj)
来源：http://bxs.yj20258.top


<!-- 参考信息 -->