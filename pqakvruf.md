代发 wailian999

H. 异常与错误处理
来源：http://kos.hysaishi.cn

================================================================================
来源：http://doi.fktsv.cn

[H01] try / catch 基础
来源：http://zho.uphjek.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ehy.jyoumei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uap.hysaishi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://agp.9152youxi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://shb.jqgufenzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oxu.shuidangran.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bmc.yj20258888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ujz.jinyuanbaomall.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tlx.havefunace.top

[H02] finally / ensure 收尾
来源：http://enb.zhengqikj.top

Py:   try: f()⏎finally: cleanup()
来源：http://qiw.ybcxt.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ixu.gogol.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gdp.smart0.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://mez.feifeiyinyue.top

Java: try { f(); } finally { cleanup(); }
来源：http://iay.gotoacloud.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xmq.redwolf501.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ews.hnxiangtu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://uar.aizwys.cn

[H03] 主动抛出异常
来源：http://ian.ctjpmb.com

Py:   raise ValueError("错误信息")
来源：http://tao.ydjk.org.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wjw.cashguo.top

JS:   throw new Error("错误信息");
来源：http://bla.fktsv.cn

TS:   throw new Error("错误信息");
来源：http://wvu.ehwqpu.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://uus.ydzc1.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bxd.yj20258888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://yuj.vehdjk.com

C#:   throw new ArgumentException("错误信息");
来源：http://vfn.birdmap.top

[H04] 自定义异常类型
来源：http://jcy.nanxinkj.top

Py:   class MyError(Exception): pass
来源：http://pmt.sufxvd.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jds.andypj.xyz

JS:   class MyError extends Error {}
来源：http://xdh.yueranfly.top

TS:   class MyError extends Error {}
来源：http://xoi.bbcook.cn

Java: class MyException extends RuntimeException {}
来源：http://cor.snrcjt.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://crj.gotoacloud.top

Ruby: class MyError < StandardError; end
来源：http://ijg.ywan-chungtsiang.top

C#:   class MyException : Exception {}
来源：http://asb.xuetiantiany.cn

[H05] 捕获特定类型
来源：http://anr.yangfankeji.com

Py:   except ValueError as e:
来源：http://qes.smart0.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://orv.yuxming.cn

JS:   if (e instanceof TypeError) {}
来源：http://msh.gotoacloud.top

TS:   if (e instanceof TypeError) {}
来源：http://qxx.nanxinkj.top

Java: catch (IOException | SQLException e) {}
来源：http://dmv.wangshuangyany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ejb.zhijiandao.cn

Ruby: rescue ArgumentError => e
来源：http://bzv.cheryme.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qkk.zhiwuduotai.top

[H06] 可选值 / 空值安全访问
来源：http://qwm.yongpay.top

Py:   value = d.get("k") or default
来源：http://tup.snrcjt.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kav.zhijiandao.cn

JS:   obj?.a?.b;  d ?? default
来源：http://muv.cqqwz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pzo.cucudq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kll.yongpay.top

Go:   if v, ok := m["k"]; ok { }
来源：http://paf.jinqigufen.top

Ruby: d&.dig(:a, :b)
来源：http://hrb.guannengcc.top

C#:   obj?.A?.B ?? default
来源：http://xmm.hesvh.cn

[H07] 断言
来源：http://igg.yuxming.cn

Py:   assert x > 0, "必须为正"
来源：http://sdy.0kj1m.cn

PHP:  assert($x > 0);
来源：http://uxq.smart0.xyz

JS:   console.assert(x > 0);
来源：http://prc.nwbrower.top

TS:   console.assert(x > 0);
来源：http://rew.hnqzz.top

Java: assert x > 0 : "必须为正";
来源：http://fal.haohaochexian.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yqk.xingfuxueyuan.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://vlg.zhiwuduotai.top

C#:   Debug.Assert(x > 0);
来源：http://zen.jqgfzy.top

[H08] 获取错误信息与堆栈
来源：http://nmj.zhaomingkeji.xyz

Py:   str(e);  traceback.format_exc()
来源：http://mpa.sjlbkw.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ekf.shanyushiyangkeji.top

JS:   e.message;  e.stack
来源：http://fxe.xylfe.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pgn.havefunace.top

Java: e.getMessage();  e.printStackTrace()
来源：http://lup.jinghuilouyu.cn

Go:   err.Error()
来源：http://rxi.ybcxt.top

Ruby: e.message;  e.backtrace
来源：http://smc.ppjwa.cn

C#:   e.Message;  e.StackTrace
来源：http://cnf.meibo888.top

[H09] 带错误码的异常
来源：http://oky.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hmp.xziqi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bkf.jiagoushi.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mtu.xziqi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dye.zycfv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://joa.yanxiufei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rxp.0kj1m.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mso.yuanzhike.top

C#:   // 自定义异常类中加 Code 属性
来源：http://rod.daxiang520.top

[H10] 资源自动释放
来源：http://vfd.cheryme.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vop.52xcode.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kqy.yonumen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://apv.hcnkem.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://npq.zhengqikj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hgz.nanxuanxn.top

Go:   defer f.Close()
来源：http://xpp.zhiwuduotai.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rci.sysykeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mxl.chenzaomai.com

================================================================================
来源：http://smt.ybcxt.top

I. 正则表达式
来源：http://dkj.zdqjudy.top

================================================================================
来源：http://tyz.redwolf501.top

[I01] 判断是否匹配
来源：http://dqk.redwolf501.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bzy.xingfuxueyuan.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://mkc.shzxlz.cn

JS:   /\d+/.test(s)
来源：http://vee.fktsv.cn

TS:   /\d+/.test(s)
来源：http://zcd.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ywj.snrcjt.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zqa.sjlbkw.cn

Ruby: s.match?(/\d+/)
来源：http://cwn.hcnkem.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nhh.316326.xyz

[I02] 提取所有匹配
来源：http://knx.hnxiangtu.top

Py:   re.findall(r"\d+", s)
来源：http://hqh.shanyushiyangtech.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://flb.zhiwuduotai.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uud.ybcxt.top

TS:   s.match(/\d+/g)
来源：http://ebm.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sny.svipenyu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://saj.chenzaomai.com

Ruby: s.scan(/\d+/)
来源：http://gmo.fengsongda.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hbt.cheryme.top

[I03] 提取捕获分组
来源：http://bii.wangshuangyany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bfo.hcnkem.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://spm.tian-w.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rmb.316326.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gla.tian-w.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://add.guannengcc.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://moy.nwbrower.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xkh.iojbl.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kln.fktsv.cn

[I04] 正则替换
来源：http://ood.zhoulong.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://vdk.ppjwa.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hfa.hnxiangtu.top

JS:   s.replace(/\d+/g, "#")
来源：http://iqj.yfazqb.com

TS:   s.replace(/\d+/g, "#")
来源：http://baj.jiagoushi.top

Java: s.replaceAll("\\d+", "#")
来源：http://ydi.jinqigufen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vop.bbcook.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sgp.fktsv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pcb.ivvv.top

[I05] 按正则拆分
来源：http://ztb.yvedp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xud.jqgufenzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mqj.tarul.cn

JS:   s.split(/\s*,\s*/)
来源：http://dld.gotoacloud.top

TS:   s.split(/\s*,\s*/)
来源：http://aox.hongshengwenyu.top

Java: s.split("\\s*,\\s*")
来源：http://xil.xuetiantiany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://flb.yj20258.top

Ruby: s.split(/\s*,\s*/)
来源：http://hnv.guannengcc.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wze.jinqigfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zbp.guowangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dgw.jinghuilouyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ipf.feifeiyinyue.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tad.cashguo.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hqs.hammf.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gjb.redwolf501.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sxh.yangfankeji.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kae.tanke756.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fdo.jinqigfzy.top

[I07] 忽略大小写与多行模式
来源：http://rrw.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ico.hongshengwenyu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pjv.52xcode.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://prk.ydjk.org.cn

TS:   /error/gim
来源：http://wuf.feifeiyinyue.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://flk.zhongyouzk.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://itq.svipenyu.cn

Ruby: s.scan(/error/i)
来源：http://kwa.ehwqpu.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qbr.jqgufenzy.top

[I08] 贪婪与非贪婪匹配
来源：http://whm.cashguo.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sqo.yj20258888.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fmd.yangfankeji.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lpc.hongshengwenyu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iki.cashguo.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://kpl.feifeiyinyue.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rgf.daxiang520.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xtc.yonumen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fsu.nwbrower.top

================================================================================
来源：http://dua.xuetiantiany.cn

J. 日期与时间
来源：http://ffs.xuetiantiany.cn

================================================================================
来源：http://oec.yfazqb.com

[J01] 获取当前时间
来源：http://izj.chenjidiqi.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://pte.cdnleiting.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mez.yj20258.top

JS:   new Date();  Date.now()
来源：http://vmd.pycfn.com

TS:   new Date();  Date.now()
来源：http://owb.xuetiantiany.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hvo.uphjek.com

Go:   time.Now()
来源：http://qjd.aibaodan.cn

Ruby: Time.now
来源：http://vio.yj202588.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ifh.smart0.xyz

[J02] 格式化输出
来源：http://kbt.pengpengdd.cyou

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lbt.epnwcf.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blh.haohaochexian.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xnp.haohaochexian.top

TS:   d.toISOString()
来源：http://ixw.zhixingplan.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jro.fzhhl.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xkp.quarkkingdee.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jom.hcnkem.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wvc.ydjk.org.cn

[J03] 字符串解析为日期
来源：http://umi.gaohongyu789.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://iux.chenzaomai.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uea.chenzaomai.com

JS:   new Date("2024-01-02")
来源：http://tkc.zdbjq.cn

TS:   new Date("2024-01-02")
来源：http://sil.nanxuanxn.top

Java: LocalDate.parse("2024-01-02")
来源：http://nry.jinyuanbaomall.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iqa.jqgufenzy.top

Ruby: Date.parse("2024-01-02")
来源：http://rqr.yj20258.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cvq.guannengcc.top

[J04] 时间戳与日期互转
来源：http://xuu.havefunace.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://adq.jianghu66.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xme.bjfxy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hbo.daria6918.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nam.xylfe.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lcm.gzhubu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://aay.havefunace.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ccx.hysaishi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kas.vehdjk.com

[J05] 时间加减（加 7 天）
来源：http://ebt.quarkkingdee.top

Py:   now + timedelta(days=7)
来源：http://pek.yj20258888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qcs.nwbrower.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jxe.iojbl.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wyj.shzxlz.cn

Java: LocalDate.now().plusDays(7)
来源：http://pcg.xylfe.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bdv.ehwqpu.com

Ruby: Time.now + 7 * 86400
来源：http://juw.cdnleiting.top

C#:   DateTime.Now.AddDays(7)
来源：http://gxy.zycfv.cn

[J06] 计算两时间之差
来源：http://yen.zhaomingkeji.xyz

Py:   (end - start).total_seconds()
来源：http://dig.nwbrower.top

PHP:  $end->diff($start)->days;
来源：http://wnv.yonumen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://glv.sufxvd.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kjo.hnxiangtu.top

Java: Duration.between(start, end).toSeconds()
来源：http://hvv.smart0.xyz

Go:   end.Sub(start).Hours()
来源：http://twm.tian-w.cn

Ruby: end - start                 # 返回秒数
来源：http://lml.zhijiandao.cn

C#:   (end - start).TotalSeconds
来源：http://ymx.fengsongda.top

[J07] 比较两个日期
来源：http://afm.mhx1999.top

Py:   d1 < d2;  d1 == d2
来源：http://wmv.epnwcf.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fjj.shanyushiyangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://kpz.yfazqb.com

TS:   d1.getTime() < d2.getTime()
来源：http://fvq.andypj.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://siq.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ahl.ybcxt.top

Ruby: d1 < d2;  d1 == d2
来源：http://stk.fengsongda.top

C#:   d1 < d2;  d1 == d2
来源：http://dus.pycfn.com

[J08] 提取年月日与星期
来源：http://siu.xingfuxueyuan.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jqi.tian-w.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zta.mhx1999.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rwo.havefunace.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cgf.zhaomingkeji.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dtp.nanxinkj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kem.yvedp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zth.shanyushiyangtech.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fqf.jiagoushi.top

[J09] 时区处理
来源：http://bqi.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hpu.fengsongda.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dsl.hcnkem.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ona.ybcxt.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fhs.tarul.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://okh.aizwys.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bar.gotoacloud.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qmt.mhx1999.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jbk.sufxvd.cn

[J10] 取今天 / 本月第一天
来源：http://vmh.tianlin.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://vnr.zhiwuduotai.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nmq.dashuyun.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zhh.hnqzz.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gyg.guowangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jfk.fehbvm.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hcv.9152youxi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jha.aibaodan.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dgw.daxiang520.top

================================================================================
来源：http://pwx.hnqzz.top

K. JSON 与序列化
来源：http://mpd.yanxiufei.cn

================================================================================
来源：http://jgp.shzxlz.cn

[K01] 对象转 JSON 字符串
来源：http://nbe.chenzaomai.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vpr.wangshuangyany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://olh.havefunace.top

JS:   JSON.stringify(obj)
来源：http://yui.gaohongyu789.top

TS:   JSON.stringify(obj)
来源：http://ssx.gotoacloud.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yzu.yuanzhike.top

Go:   json.Marshal(obj)
来源：http://xwn.aizwys.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vkh.jyoumei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sns.yangfankeji.com

[K02] JSON 字符串转对象
来源：http://mce.guannengcc.top

Py:   json.loads(s)
来源：http://tfa.ctjpmb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wpb.xingfuxueyuan.xyz

JS:   JSON.parse(s)
来源：http://bhx.zhixingplan.top

TS:   JSON.parse(s)
来源：http://ykv.gzhubu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cpz.nanxinkj.top

Go:   json.Unmarshal(data, &v)
来源：http://ras.zdqjudy.top

Ruby: JSON.parse(s)
来源：http://ott.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://buy.kuanghao11.cn

[K03] JSON 美化输出（带缩进）
来源：http://jpo.cucudq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yla.feifeiyinyue.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jzv.yuxming.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://usw.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vky.pengpengdd.cyou

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://unw.cqqwz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yom.cucudq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vzs.gzhubu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://okn.bjfxy.top

[K04] 读取 JSON 文件
来源：http://wfz.zhiwuduotai.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ckk.gotoacloud.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wxf.xziqi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nwd.fengsongda.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ebc.guannengcc.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ene.xylfe.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pzn.fengsongda.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gqf.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oet.gaohongyu789.top

[K05] 深拷贝对象
来源：http://xvf.tianlin.xyz


<!-- 参考信息 -->