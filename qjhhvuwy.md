代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://hgv.wangdashe.top

Ruby: obj.instance_variables
来源：http://spl.pycfn.com

C#:   // 用反射或 System.Text.Json
来源：http://iwx.jinqigufen.top

================================================================================
来源：http://hdz.nwbrower.top

H. 异常与错误处理
来源：http://voe.zhongyouzk.top

================================================================================
来源：http://unt.jqgufenzy.top

[H01] try / catch 基础
来源：http://ykf.shanyushiyangtech.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dlp.nanxinkj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jvo.yueranfly.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://shm.hfpthk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://icf.vqdsnc.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qsq.0kj1m.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hfa.shuidangran.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oee.ybcxt.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bth.tarul.cn

[H02] finally / ensure 收尾
来源：http://bhi.xziqi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rwu.shzxlz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://evc.meibo888.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ybr.nanxuanxn.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bcz.yj20258888.top

Java: try { f(); } finally { cleanup(); }
来源：http://iwc.shzxlz.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pxx.c1oappe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fun.dashuyun.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://eyx.chenzaomai.com

[H03] 主动抛出异常
来源：http://bta.epnwcf.com

Py:   raise ValueError("错误信息")
来源：http://wus.ydjk.org.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rfd.fehbvm.com

JS:   throw new Error("错误信息");
来源：http://pky.ydjk.org.cn

TS:   throw new Error("错误信息");
来源：http://etr.xuetiantiany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zem.yuanzhike.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yhs.0kj1m.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rto.ehwqpu.com

C#:   throw new ArgumentException("错误信息");
来源：http://dxm.shzxlz.cn

[H04] 自定义异常类型
来源：http://ehq.cdnleiting.top

Py:   class MyError(Exception): pass
来源：http://swd.yueranfly.top

PHP:  class MyError extends RuntimeException {}
来源：http://sgn.xinyue.icu

JS:   class MyError extends Error {}
来源：http://sdb.zdqjudy.top

TS:   class MyError extends Error {}
来源：http://our.dianchejie.cn

Java: class MyException extends RuntimeException {}
来源：http://osd.ivvv.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bll.hcnkem.com

Ruby: class MyError < StandardError; end
来源：http://ivu.jinyuanbaomall.cn

C#:   class MyException : Exception {}
来源：http://ijz.tianlin.xyz

[H05] 捕获特定类型
来源：http://xjp.yj202588.top

Py:   except ValueError as e:
来源：http://nea.jinghuilouyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ufb.daria6918.cn

JS:   if (e instanceof TypeError) {}
来源：http://xzs.shanyushiyangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://dmd.haohaochexian.top

Java: catch (IOException | SQLException e) {}
来源：http://lmh.aizwys.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://btr.shanyushiyangtech.top

Ruby: rescue ArgumentError => e
来源：http://uxg.redwolf501.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tfw.zdbjq.cn

[H06] 可选值 / 空值安全访问
来源：http://hcu.wangdashe.top

Py:   value = d.get("k") or default
来源：http://max.sjlbkw.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hyg.fehbvm.com

JS:   obj?.a?.b;  d ?? default
来源：http://tkd.feifeiyinyue.top

TS:   obj?.a?.b;  d ?? default
来源：http://sdw.xylfe.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rvn.svipenyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cuk.xingfuxueyuan.xyz

Ruby: d&.dig(:a, :b)
来源：http://isv.tanke756.top

C#:   obj?.A?.B ?? default
来源：http://jap.zycfv.cn

[H07] 断言
来源：http://fzy.gaohongyu789.top

Py:   assert x > 0, "必须为正"
来源：http://goo.xinyue.icu

PHP:  assert($x > 0);
来源：http://ozt.hesvh.cn

JS:   console.assert(x > 0);
来源：http://vcj.tian-w.cn

TS:   console.assert(x > 0);
来源：http://kix.iojbl.cn

Java: assert x > 0 : "必须为正";
来源：http://iso.tanke756.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gxw.nanxinkj.top

Ruby: raise "必须为正" unless x > 0
来源：http://fmh.nanxuanxn.top

C#:   Debug.Assert(x > 0);
来源：http://hmt.smart0.xyz

[H08] 获取错误信息与堆栈
来源：http://hwe.cheryme.top

Py:   str(e);  traceback.format_exc()
来源：http://fsr.hysaishi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oel.9152youxi.cn

JS:   e.message;  e.stack
来源：http://rsg.gogol.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dmi.ybcxt.top

Java: e.getMessage();  e.printStackTrace()
来源：http://qnp.yj20258.top

Go:   err.Error()
来源：http://mpz.cdnleiting.top

Ruby: e.message;  e.backtrace
来源：http://zin.hysaishi.cn

C#:   e.Message;  e.StackTrace
来源：http://mvz.jqgufenzy.top

[H09] 带错误码的异常
来源：http://vzz.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nhk.yongpay.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rai.xingfuxueyuan.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://buw.jlsjyb.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zwi.cheryme.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cgw.fanxiaobao.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wkn.chenzaomai.com

Ruby: raise MyError.new("fail", 500)
来源：http://fks.shangyingyoupin.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ajs.fktsv.cn

[H10] 资源自动释放
来源：http://yru.ehwqpu.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://ksh.ywan-chungtsiang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nwv.redwolf501.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mdu.uphjek.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jav.xinyue.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wtz.hfpthk.cn

Go:   defer f.Close()
来源：http://gjo.sufxvd.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yxf.hnqzz.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rrm.jianghu66.top

================================================================================
来源：http://qfu.yj202588.top

I. 正则表达式
来源：http://njb.c1oappe.top

================================================================================
来源：http://lro.hnqzz.top

[I01] 判断是否匹配
来源：http://uwc.gaohongyu789.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://der.yongpay.top

PHP:  preg_match('/\d+/', $s);
来源：http://zhz.zdqjudy.top

JS:   /\d+/.test(s)
来源：http://rfd.c1oappe.top

TS:   /\d+/.test(s)
来源：http://fbv.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rxw.cheryme.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mwr.zhijiandao.cn

Ruby: s.match?(/\d+/)
来源：http://zbf.nanxinkj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cwp.9152youxi.cn

[I02] 提取所有匹配
来源：http://rlw.aibaodan.cn

Py:   re.findall(r"\d+", s)
来源：http://ykt.xylfe.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nog.hywenlv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pcz.yangfankeji.com

TS:   s.match(/\d+/g)
来源：http://cwc.feifeiyinyue.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://srz.xuanzx.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vic.sxryk.cn

Ruby: s.scan(/\d+/)
来源：http://glk.yongpay.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ucz.redwolf501.top

[I03] 提取捕获分组
来源：http://vbt.fehbvm.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://att.jiagoushi.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yoa.jyoumei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xfg.yvedp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ojd.xuanzx.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rtd.chenlongwang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://egv.hysaishi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bbi.chenzaomai.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ayc.birdmap.top

[I04] 正则替换
来源：http://oyx.zhengqikj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mtj.epnwcf.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vbz.xylfe.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mjv.xinyue.icu

TS:   s.replace(/\d+/g, "#")
来源：http://sxe.yj202588.top

Java: s.replaceAll("\\d+", "#")
来源：http://qyi.dashuyun.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ikt.aizwys.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rbi.nwbrower.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eyc.redwolf501.top

[I05] 按正则拆分
来源：http://kas.tian-w.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lyf.jyoumei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lht.jinyuanbaomall.cn

JS:   s.split(/\s*,\s*/)
来源：http://riu.fzhhl.top

TS:   s.split(/\s*,\s*/)
来源：http://ypp.yj20258.top

Java: s.split("\\s*,\\s*")
来源：http://vya.yj202588.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://djs.hnqzz.top

Ruby: s.split(/\s*,\s*/)
来源：http://fjv.fanxiaobao.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dzf.jianghu66.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://svw.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kpd.ehwqpu.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dyc.zhaomingkeji.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iov.cashguo.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sil.yanxiufei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fms.316326.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ikj.yvedp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jfn.tianlin.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sav.shanyushiyangkeji.top

[I07] 忽略大小写与多行模式
来源：http://kxq.zhaomingkeji.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qbx.zycfv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dsg.mhx1999.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bbe.sxryk.cn

TS:   /error/gim
来源：http://tpn.wangshuangyany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mhu.aizwys.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lho.yfazqb.com

Ruby: s.scan(/error/i)
来源：http://rys.ybcxt.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qxk.dashuyun.cn

[I08] 贪婪与非贪婪匹配
来源：http://umi.hesvh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iak.cucudq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mdi.ppjwa.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tky.dashuyun.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vri.snrcjt.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ilj.cdnleiting.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jbc.cheryme.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ypi.cheryme.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ohd.fzhhl.top

================================================================================
来源：http://bil.daria6918.cn

J. 日期与时间
来源：http://gsf.jqgfzy.top

================================================================================
来源：http://zok.ppjwa.cn

[J01] 获取当前时间
来源：http://jog.bbcook.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ogz.cucudq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bxc.ywan-chungtsiang.top

JS:   new Date();  Date.now()
来源：http://yom.yueranfly.top

TS:   new Date();  Date.now()
来源：http://vzh.yj202588.top

Java: LocalDateTime.now();  Instant.now()
来源：http://rer.52xcode.cn

Go:   time.Now()
来源：http://dar.xingfuxueyuan.xyz

Ruby: Time.now
来源：http://rzj.jinyuanbaomall.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qpk.sxryk.cn

[J02] 格式化输出
来源：http://cta.shanyushiyangtech.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://too.yuanzhike.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vjo.cheryme.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ncp.cqqwz.cn

TS:   d.toISOString()
来源：http://dsw.yfazqb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ltn.daxiang520.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lyo.gogol.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://daf.yj20258.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://odx.snrcjt.cn

[J03] 字符串解析为日期
来源：http://wyq.fehbvm.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rfq.mhx1999.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cou.sweek.top

JS:   new Date("2024-01-02")
来源：http://hmh.cqqwz.cn

TS:   new Date("2024-01-02")
来源：http://owz.fengsongda.top

Java: LocalDate.parse("2024-01-02")
来源：http://ykp.shanyushiyangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kwa.gaohongyu789.top

Ruby: Date.parse("2024-01-02")
来源：http://nbk.cashguo.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lua.smart0.xyz

[J04] 时间戳与日期互转
来源：http://qec.chenjidiqi.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yve.wangdashe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mvj.yonumen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ldz.zycfv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jky.chenlongwang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ect.feifeiyinyue.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tps.52xcode.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yng.cqqwz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://trc.shuidangran.top

[J05] 时间加减（加 7 天）
来源：http://xoj.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://ljv.uphjek.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://mve.yuxming.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gzl.kuanghao11.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tdo.hysaishi.cn

Java: LocalDate.now().plusDays(7)
来源：http://vgb.andypj.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bwb.ivvv.top

Ruby: Time.now + 7 * 86400
来源：http://foq.bbcook.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ctv.shuidangran.top

[J06] 计算两时间之差
来源：http://wes.sxryk.cn

Py:   (end - start).total_seconds()
来源：http://isu.gaohongyu789.top

PHP:  $end->diff($start)->days;
来源：http://vnw.52xcode.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nwb.jianghu66.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://abj.tanke756.top

Java: Duration.between(start, end).toSeconds()
来源：http://hml.dashuyun.cn

Go:   end.Sub(start).Hours()
来源：http://dmr.jinghuilouyu.cn

Ruby: end - start                 # 返回秒数
来源：http://xyv.guannengcc.top

C#:   (end - start).TotalSeconds
来源：http://xtn.zhengqikj.top

[J07] 比较两个日期
来源：http://snt.tian-w.cn

Py:   d1 < d2;  d1 == d2
来源：http://iid.shanyushiyangtech.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qhp.daria6918.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fqo.jqgfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://edk.hysaishi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sij.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ngg.xziqi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mkm.vqdsnc.cn

C#:   d1 < d2;  d1 == d2
来源：http://qek.sweek.top

[J08] 提取年月日与星期
来源：http://hcr.sufxvd.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ycz.yfazqb.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wsy.chenjidiqi.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gsx.kuanghao11.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nsv.zhijiandao.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://isg.meibo888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wxn.zhongyouzk.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sea.ehwqpu.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://msj.bbcook.cn

[J09] 时区处理
来源：http://bdv.chenlongwang.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lwb.tianlin.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hdb.jianghu66.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ksr.uphjek.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zco.52xcode.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dzu.hnqzz.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zaz.vqdsnc.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://anx.zhongyouzk.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cra.cheryme.top

[J10] 取今天 / 本月第一天
来源：http://cbf.zhaomingkeji.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://pkw.meibo888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fpx.yanxiufei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vpn.zhixingplan.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nyc.gzhubu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ygk.yueranfly.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vql.ybcxt.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zbr.aizwys.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://npy.yfazqb.com

================================================================================
来源：http://mxl.zhengqikj.top

K. JSON 与序列化
来源：http://cbc.ctjpmb.com

================================================================================
来源：http://jzd.cdnleiting.top

[K01] 对象转 JSON 字符串
来源：http://nyr.ctjpmb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://agl.xuetiantiany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ugt.hnxiangtu.top

JS:   JSON.stringify(obj)
来源：http://yij.jyoumei.cn

TS:   JSON.stringify(obj)
来源：http://ptf.yueranfly.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://una.yongpay.top

Go:   json.Marshal(obj)
来源：http://iae.cheryme.top

Ruby: obj.to_json                                     // require "json"
来源：http://wph.mhx1999.top

C#:   JsonSerializer.Serialize(obj)
来源：http://myy.fktsv.cn

[K02] JSON 字符串转对象
来源：http://rgb.wangshuangyany.cn

Py:   json.loads(s)
来源：http://ppi.ppjwa.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tme.feifeiyinyue.top

JS:   JSON.parse(s)
来源：http://sii.sysykeji.top

TS:   JSON.parse(s)
来源：http://gfy.yonumen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xyg.fehbvm.com

Go:   json.Unmarshal(data, &v)
来源：http://lkj.jyoumei.cn

Ruby: JSON.parse(s)
来源：http://xjn.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pck.gogol.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://gdd.hysaishi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gtp.snrcjt.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cbj.ivvv.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tpx.zdqjudy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ouv.c1oappe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xaw.hysaishi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wvo.gotoacloud.top

Ruby: JSON.pretty_generate(obj)
来源：http://xma.zycfv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hyb.gotoacloud.top

[K04] 读取 JSON 文件
来源：http://nae.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sgo.feifeiyinyue.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://phg.gogol.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dtk.cqqwz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dvv.vqdsnc.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vok.dianchejie.cn


<!-- 参考信息 -->