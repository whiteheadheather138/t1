代发 wailian999

PHP:  get_object_vars($obj);
来源：http://vjf.guowangkeji.top

JS:   Object.entries(obj)
来源：http://txu.52xcode.cn

TS:   Object.entries(obj)
来源：http://jvr.fehbvm.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bgg.yj20258888.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fam.gotoacloud.top

Ruby: obj.instance_variables
来源：http://jwx.9152youxi.cn

C#:   // 用反射或 System.Text.Json
来源：http://yjj.ppjwa.cn

================================================================================
来源：http://dck.hnxiangtu.top

H. 异常与错误处理
来源：http://qof.dianchejie.cn

================================================================================
来源：http://xys.hnxiangtu.top

[H01] try / catch 基础
来源：http://tir.gotoacloud.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fyl.yanxiufei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pue.jinqigufen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fri.hfpthk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xdv.svipenyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uvm.hcnkem.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uzc.cheryme.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nox.sufxvd.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nai.cdnleiting.top

[H02] finally / ensure 收尾
来源：http://tcn.zhijiandao.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kaa.hongshengwenyu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ajc.quarkkingdee.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rps.hongshengwenyu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nir.vqdsnc.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bvw.jiagoushi.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bok.zhaomingkeji.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://ibe.jinqigfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ujb.yangfankeji.com

[H03] 主动抛出异常
来源：http://kzp.hcnkem.com

Py:   raise ValueError("错误信息")
来源：http://gae.bjfxy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://orp.hywenlv.cn

JS:   throw new Error("错误信息");
来源：http://ltw.birdmap.top

TS:   throw new Error("错误信息");
来源：http://jqs.wangdashe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://sib.quarkkingdee.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nix.guannengcc.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ici.svipenyu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pse.svipenyu.cn

[H04] 自定义异常类型
来源：http://ryz.nanxinkj.top

Py:   class MyError(Exception): pass
来源：http://ydh.fktsv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hjc.fktsv.cn

JS:   class MyError extends Error {}
来源：http://udb.havefunace.top

TS:   class MyError extends Error {}
来源：http://njp.52xcode.cn

Java: class MyException extends RuntimeException {}
来源：http://llq.zhaomingkeji.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ifm.ywan-chungtsiang.top

Ruby: class MyError < StandardError; end
来源：http://jta.snrcjt.cn

C#:   class MyException : Exception {}
来源：http://xyb.bjfxy.top

[H05] 捕获特定类型
来源：http://zhe.hnxiangtu.top

Py:   except ValueError as e:
来源：http://hbg.ydzc1.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://paw.zhiwuduotai.top

JS:   if (e instanceof TypeError) {}
来源：http://lpw.sysykeji.top

TS:   if (e instanceof TypeError) {}
来源：http://uvl.daxiang520.top

Java: catch (IOException | SQLException e) {}
来源：http://vaq.ybcxt.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gqe.birdmap.top

Ruby: rescue ArgumentError => e
来源：http://oxf.gogol.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pfn.hammf.cn

[H06] 可选值 / 空值安全访问
来源：http://ouf.jyoumei.cn

Py:   value = d.get("k") or default
来源：http://efw.hammf.cn

PHP:  $v = $d["k"] ?? null;
来源：http://isu.guowangkeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://kdf.fanxiaobao.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://vip.guannengcc.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pos.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jpf.gzhubu.top

Ruby: d&.dig(:a, :b)
来源：http://wmo.hcnkem.com

C#:   obj?.A?.B ?? default
来源：http://wow.pengpengdd.cyou

[H07] 断言
来源：http://awl.zdqjudy.top

Py:   assert x > 0, "必须为正"
来源：http://nmw.shanyushiyangtech.top

PHP:  assert($x > 0);
来源：http://bec.yanxiufei.cn

JS:   console.assert(x > 0);
来源：http://mkc.jiagoushi.top

TS:   console.assert(x > 0);
来源：http://ncn.tianlin.xyz

Java: assert x > 0 : "必须为正";
来源：http://ohw.guannengcc.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yiq.chenzaomai.com

Ruby: raise "必须为正" unless x > 0
来源：http://lhz.hnxiangtu.top

C#:   Debug.Assert(x > 0);
来源：http://qwc.316326.xyz

[H08] 获取错误信息与堆栈
来源：http://qmx.chenzaomai.com

Py:   str(e);  traceback.format_exc()
来源：http://zhi.vqdsnc.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xdm.daxiang520.top

JS:   e.message;  e.stack
来源：http://iri.yanxiufei.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lpe.zdbjq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pst.shangyingyoupin.top

Go:   err.Error()
来源：http://loq.yuxming.cn

Ruby: e.message;  e.backtrace
来源：http://hqh.jinyuanbaomall.cn

C#:   e.Message;  e.StackTrace
来源：http://mdc.gogol.net.cn

[H09] 带错误码的异常
来源：http://mcg.yanxiufei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uvs.c1oappe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fxp.hysaishi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uds.gaohongyu789.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fqf.xingfuxueyuan.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hym.ybcxt.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wjs.yueranfly.top

Ruby: raise MyError.new("fail", 500)
来源：http://mhj.feifeiyinyue.top

C#:   // 自定义异常类中加 Code 属性
来源：http://mce.yanxiufei.cn

[H10] 资源自动释放
来源：http://gto.wangdashe.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://coi.ppjwa.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fup.fehbvm.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mzj.wangshuangyany.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mml.aibaodan.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rmk.haohaochexian.top

Go:   defer f.Close()
来源：http://iko.ybcxt.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ibb.quarkkingdee.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://aqv.sufxvd.cn

================================================================================
来源：http://qak.wangdashe.top

I. 正则表达式
来源：http://jgj.shanyushiyangtech.top

================================================================================
来源：http://kic.yonumen.top

[I01] 判断是否匹配
来源：http://rhs.sweek.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dpa.bjfxy.top

PHP:  preg_match('/\d+/', $s);
来源：http://ldl.pengpengdd.cyou

JS:   /\d+/.test(s)
来源：http://jsi.fehbvm.com

TS:   /\d+/.test(s)
来源：http://eaa.sweek.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kxs.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wtv.aizwys.cn

Ruby: s.match?(/\d+/)
来源：http://yma.tanke756.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://edy.gaohongyu789.top

[I02] 提取所有匹配
来源：http://kup.cucudq.cn

Py:   re.findall(r"\d+", s)
来源：http://cqt.shangyingyoupin.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ydw.aizwys.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ohf.52xcode.cn

TS:   s.match(/\d+/g)
来源：http://wru.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nkk.yj202588.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hcs.shzxlz.cn

Ruby: s.scan(/\d+/)
来源：http://pyl.zhiwuduotai.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cqj.bjfxy.top

[I03] 提取捕获分组
来源：http://cbp.pycfn.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sag.zhixingplan.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oau.yonumen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://aho.guowangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lnq.gogol.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://arc.yj20258888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uqz.hnqzz.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jaw.hywenlv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xoy.smart0.xyz

[I04] 正则替换
来源：http://kxn.xuanzx.com

Py:   re.sub(r"\d+", "#", s)
来源：http://vbg.jyoumei.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tnx.cheryme.top

JS:   s.replace(/\d+/g, "#")
来源：http://bqc.guowangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://pjx.yuxming.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rsf.vqdsnc.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://igi.bbcook.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ciy.wangshuangyany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eot.vqdsnc.cn

[I05] 按正则拆分
来源：http://hjj.mhx1999.top

Py:   re.split(r"\s*,\s*", s)
来源：http://dvi.sjlbkw.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://neb.mhx1999.top

JS:   s.split(/\s*,\s*/)
来源：http://btm.hammf.cn

TS:   s.split(/\s*,\s*/)
来源：http://zik.aizwys.cn

Java: s.split("\\s*,\\s*")
来源：http://vqg.yuxming.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sil.dianchejie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wtw.zhijiandao.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ttx.nanxinkj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lat.hywenlv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pin.jqgfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vgp.feifeiyinyue.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://upt.shanyushiyangtech.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://epi.hesvh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uxx.nanxuanxn.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gzs.ydjk.org.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yrn.nanxinkj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lff.hnxiangtu.top

[I07] 忽略大小写与多行模式
来源：http://ave.tarul.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xdl.hesvh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://faf.tianlin.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://irt.shuidangran.top

TS:   /error/gim
来源：http://ull.ctjpmb.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://elf.jinyuanbaomall.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ptn.chenjidiqi.icu

Ruby: s.scan(/error/i)
来源：http://xwd.zdbjq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vzm.yj20258.top

[I08] 贪婪与非贪婪匹配
来源：http://jax.shanyushiyangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://njs.yongpay.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tva.yanxiufei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://glb.zdbjq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://etw.jinghuilouyu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qwv.fengsongda.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qqr.jiagoushi.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://izm.yueranfly.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yuo.aibaodan.cn

================================================================================
来源：http://nst.hcnkem.com

J. 日期与时间
来源：http://lnk.sjlbkw.cn

================================================================================
来源：http://kti.chenlongwang.top

[J01] 获取当前时间
来源：http://xju.shangyingyoupin.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wme.aizwys.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yhb.tanke756.top

JS:   new Date();  Date.now()
来源：http://hxs.hongshengwenyu.top

TS:   new Date();  Date.now()
来源：http://zdb.pengpengdd.cyou

Java: LocalDateTime.now();  Instant.now()
来源：http://lly.gaohongyu789.top

Go:   time.Now()
来源：http://kmh.sysykeji.top

Ruby: Time.now
来源：http://jql.birdmap.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uvl.ydjk.org.cn

[J02] 格式化输出
来源：http://idq.quarkkingdee.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jct.yj202588.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vdc.ybcxt.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iyl.zhijiandao.cn

TS:   d.toISOString()
来源：http://obt.sjlbkw.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jjo.gzhubu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ygy.jlsjyb.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://keb.yongpay.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ahd.tanke756.top

[J03] 字符串解析为日期
来源：http://njv.yongpay.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://iln.ehwqpu.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://syj.epnwcf.com

JS:   new Date("2024-01-02")
来源：http://snz.c1oappe.top

TS:   new Date("2024-01-02")
来源：http://psr.nanxinkj.top

Java: LocalDate.parse("2024-01-02")
来源：http://hds.shanyushiyangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://btp.dashuyun.cn

Ruby: Date.parse("2024-01-02")
来源：http://odf.316326.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hac.nanxinkj.top

[J04] 时间戳与日期互转
来源：http://fqt.yj20258888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tds.zhixingplan.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mst.jqgfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wcc.hesvh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wdq.hesvh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xqw.feifeiyinyue.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oux.quarkkingdee.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cux.yj20258.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ujt.nanxuanxn.top

[J05] 时间加减（加 7 天）
来源：http://unc.ydjk.org.cn

Py:   now + timedelta(days=7)
来源：http://rnf.havefunace.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://quh.vehdjk.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qbg.meibo888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rcq.dashuyun.cn

Java: LocalDate.now().plusDays(7)
来源：http://kux.yangfankeji.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eju.svipenyu.cn

Ruby: Time.now + 7 * 86400
来源：http://oii.xinyue.icu

C#:   DateTime.Now.AddDays(7)
来源：http://gob.tianlin.xyz

[J06] 计算两时间之差
来源：http://qqm.shangyingyoupin.top

Py:   (end - start).total_seconds()
来源：http://imi.snrcjt.cn

PHP:  $end->diff($start)->days;
来源：http://sds.ydjk.org.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hai.xingfuxueyuan.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lhw.hnqzz.top

Java: Duration.between(start, end).toSeconds()
来源：http://cjp.zhijiandao.cn

Go:   end.Sub(start).Hours()
来源：http://eoy.feifeiyinyue.top

Ruby: end - start                 # 返回秒数
来源：http://ofx.meibo888.top

C#:   (end - start).TotalSeconds
来源：http://wrb.yj202588.top

[J07] 比较两个日期
来源：http://vzm.fengsongda.top

Py:   d1 < d2;  d1 == d2
来源：http://igd.sysykeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://djs.xylfe.cn

JS:   d1.getTime() < d2.getTime()
来源：http://koc.cheryme.top

TS:   d1.getTime() < d2.getTime()
来源：http://wbt.zdbjq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yqf.tanke756.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fdl.zdqjudy.top

Ruby: d1 < d2;  d1 == d2
来源：http://izr.wangshuangyany.cn

C#:   d1 < d2;  d1 == d2
来源：http://oxw.sufxvd.cn

[J08] 提取年月日与星期
来源：http://xhp.shanyushiyangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://njz.svipenyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sdi.shuidangran.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yez.gotoacloud.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rye.hesvh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hbs.yuxming.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xvd.bjfxy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oqd.yuanzhike.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kgp.smart0.xyz

[J09] 时区处理
来源：http://zzw.0kj1m.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jkf.yj202588.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ljx.hammf.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nyf.fzhhl.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gvy.bjfxy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tmr.zdbjq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qbw.chenzaomai.com

Ruby: Time.now.getlocal("+08:00")
来源：http://sxs.cashguo.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lkp.shuidangran.top

[J10] 取今天 / 本月第一天
来源：http://uko.jinqigufen.top

Py:   date.today();  date.today().replace(day=1)
来源：http://knj.yvedp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iug.xuanzx.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ewb.uphjek.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mwt.fehbvm.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jnz.fzhhl.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xcd.gotoacloud.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hvg.ywan-chungtsiang.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jly.gaohongyu789.top

================================================================================
来源：http://cpw.daxiang520.top

K. JSON 与序列化
来源：http://kdr.zhaomingkeji.xyz

================================================================================
来源：http://ptl.yfazqb.com

[K01] 对象转 JSON 字符串
来源：http://drz.jqgfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rwi.mhx1999.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zyx.pycfn.com

JS:   JSON.stringify(obj)
来源：http://zod.chenlongwang.top

TS:   JSON.stringify(obj)
来源：http://iba.andypj.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kcu.chenlongwang.top

Go:   json.Marshal(obj)
来源：http://mky.yfazqb.com

Ruby: obj.to_json                                     // require "json"
来源：http://fxx.yueranfly.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cjr.fanxiaobao.xyz

[K02] JSON 字符串转对象
来源：http://uql.quarkkingdee.top

Py:   json.loads(s)
来源：http://fvh.bbcook.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gye.ydzc1.top

JS:   JSON.parse(s)
来源：http://pxi.epnwcf.com

TS:   JSON.parse(s)
来源：http://ehx.dashuyun.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jjo.zhoulong.xyz

Go:   json.Unmarshal(data, &v)
来源：http://qya.zhongyouzk.top

Ruby: JSON.parse(s)
来源：http://jlc.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nam.gzhubu.top

[K03] JSON 美化输出（带缩进）
来源：http://nnm.ybcxt.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tyx.havefunace.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lax.yfazqb.com

JS:   JSON.stringify(obj, null, 2)
来源：http://nfd.shanyushiyangkeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://tqn.jyoumei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gps.zhaomingkeji.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tja.wangshuangyany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qxw.cheryme.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hof.birdmap.top

[K04] 读取 JSON 文件
来源：http://wpo.fehbvm.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://daf.meibo888.top


<!-- 参考信息 -->