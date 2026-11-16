代发 wailian999

H. 异常与错误处理
来源：http://jkh.fzhhl.top

================================================================================
来源：http://ahw.cdnleiting.top

[H01] try / catch 基础
来源：http://eem.ehwqpu.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zil.hcnkem.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://arv.zdbjq.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vyd.cdnleiting.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://eae.52xcode.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kep.shuidangran.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iiv.tianlin.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://izr.hnqzz.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lto.shzxlz.cn

[H02] finally / ensure 收尾
来源：http://mzo.yuanzhike.top

Py:   try: f()⏎finally: cleanup()
来源：http://azk.chenlongwang.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://slm.zdqjudy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://yhj.pycfn.com

TS:   try { f(); } finally { cleanup(); }
来源：http://bbs.hcnkem.com

Java: try { f(); } finally { cleanup(); }
来源：http://qvt.zhaomingkeji.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://gqo.guowangkeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bzh.52xcode.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hgq.vehdjk.com

[H03] 主动抛出异常
来源：http://ilw.xuetiantiany.cn

Py:   raise ValueError("错误信息")
来源：http://ihc.xziqi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jeh.hcnkem.com

JS:   throw new Error("错误信息");
来源：http://mtq.vqdsnc.cn

TS:   throw new Error("错误信息");
来源：http://aup.vehdjk.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://ybs.hongshengwenyu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mgu.tanke756.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hzm.c1oappe.top

C#:   throw new ArgumentException("错误信息");
来源：http://nrx.redwolf501.top

[H04] 自定义异常类型
来源：http://kid.yongpay.top

Py:   class MyError(Exception): pass
来源：http://mfy.xuanzx.com

PHP:  class MyError extends RuntimeException {}
来源：http://aty.zhixingplan.top

JS:   class MyError extends Error {}
来源：http://oyn.smart0.xyz

TS:   class MyError extends Error {}
来源：http://yza.jqgufenzy.top

Java: class MyException extends RuntimeException {}
来源：http://rrx.fehbvm.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://opm.zhijiandao.cn

Ruby: class MyError < StandardError; end
来源：http://vml.mhx1999.top

C#:   class MyException : Exception {}
来源：http://kef.tarul.cn

[H05] 捕获特定类型
来源：http://mnj.pengpengdd.cyou

Py:   except ValueError as e:
来源：http://rpm.yj20258.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ynj.hnxiangtu.top

JS:   if (e instanceof TypeError) {}
来源：http://hoh.fengsongda.top

TS:   if (e instanceof TypeError) {}
来源：http://xtl.jqgufenzy.top

Java: catch (IOException | SQLException e) {}
来源：http://fed.tianlin.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bsu.daxiang520.top

Ruby: rescue ArgumentError => e
来源：http://ltj.sxryk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dui.xinyue.icu

[H06] 可选值 / 空值安全访问
来源：http://mxq.xinyue.icu

Py:   value = d.get("k") or default
来源：http://vhp.smart0.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://znk.xziqi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gza.yvedp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gmw.pengpengdd.cyou

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sxo.vehdjk.com

Go:   if v, ok := m["k"]; ok { }
来源：http://bwt.zhoulong.xyz

Ruby: d&.dig(:a, :b)
来源：http://lnc.tian-w.cn

C#:   obj?.A?.B ?? default
来源：http://vbt.bjfxy.top

[H07] 断言
来源：http://yht.jinyuanbaomall.cn

Py:   assert x > 0, "必须为正"
来源：http://vuc.daria6918.cn

PHP:  assert($x > 0);
来源：http://bzy.meibo888.top

JS:   console.assert(x > 0);
来源：http://seb.snrcjt.cn

TS:   console.assert(x > 0);
来源：http://uwk.vqdsnc.cn

Java: assert x > 0 : "必须为正";
来源：http://dvi.jinqigufen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yhl.gogol.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nte.zhoulong.xyz

C#:   Debug.Assert(x > 0);
来源：http://wne.jiagoushi.top

[H08] 获取错误信息与堆栈
来源：http://wft.cheryme.top

Py:   str(e);  traceback.format_exc()
来源：http://qzt.jlsjyb.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nvl.shuidangran.top

JS:   e.message;  e.stack
来源：http://tuc.shzxlz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://saw.zycfv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rpa.andypj.xyz

Go:   err.Error()
来源：http://fra.hongshengwenyu.top

Ruby: e.message;  e.backtrace
来源：http://rul.zdqjudy.top

C#:   e.Message;  e.StackTrace
来源：http://rey.yuxming.cn

[H09] 带错误码的异常
来源：http://efs.andypj.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ypz.andypj.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://frx.fanxiaobao.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eqf.nwbrower.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://goy.hnxiangtu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://exw.cdnleiting.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ldq.xuetiantiany.cn

Ruby: raise MyError.new("fail", 500)
来源：http://emz.jqgfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ewu.fehbvm.com

[H10] 资源自动释放
来源：http://zal.guannengcc.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://gyb.pengpengdd.cyou

PHP:  // 无 with：在 finally 里 fclose()
来源：http://shx.kuanghao11.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zqc.zhixingplan.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ixw.0kj1m.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pva.yongpay.top

Go:   defer f.Close()
来源：http://vcw.wangshuangyany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://igl.9152youxi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://drl.zhijiandao.cn

================================================================================
来源：http://ghx.sysykeji.top

I. 正则表达式
来源：http://wpl.sxryk.cn

================================================================================
来源：http://ivc.yanxiufei.cn

[I01] 判断是否匹配
来源：http://kqu.zhixingplan.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zmd.hesvh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jhc.zhijiandao.cn

JS:   /\d+/.test(s)
来源：http://iml.jinyuanbaomall.cn

TS:   /\d+/.test(s)
来源：http://rpz.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ior.fzhhl.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wva.sweek.top

Ruby: s.match?(/\d+/)
来源：http://vim.bjfxy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qmk.zycfv.cn

[I02] 提取所有匹配
来源：http://lro.yj202588.top

Py:   re.findall(r"\d+", s)
来源：http://jsb.nanxinkj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bfw.ivvv.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://itj.9152youxi.cn

TS:   s.match(/\d+/g)
来源：http://cmd.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xap.yvedp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tcg.tanke756.top

Ruby: s.scan(/\d+/)
来源：http://hzj.guannengcc.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pmo.feifeiyinyue.top

[I03] 提取捕获分组
来源：http://lvt.wangdashe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ovl.jqgufenzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mge.ybcxt.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sqm.chenlongwang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vaq.zhongyouzk.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://glm.bjfxy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lkg.jinghuilouyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nnu.jqgfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oub.shuidangran.top

[I04] 正则替换
来源：http://gsr.shanyushiyangtech.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hwx.snrcjt.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dgn.hnqzz.top

JS:   s.replace(/\d+/g, "#")
来源：http://psh.zycfv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qgx.fehbvm.com

Java: s.replaceAll("\\d+", "#")
来源：http://pga.snrcjt.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ssz.vehdjk.com

Ruby: s.gsub(/\d+/, "#")
来源：http://ecu.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ggd.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://ubf.jyoumei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://etm.jqgfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dhw.zdqjudy.top

JS:   s.split(/\s*,\s*/)
来源：http://bqt.xylfe.cn

TS:   s.split(/\s*,\s*/)
来源：http://nxr.yongpay.top

Java: s.split("\\s*,\\s*")
来源：http://dah.jinghuilouyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sqp.svipenyu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nww.guannengcc.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pih.fengsongda.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oqd.smart0.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xal.vehdjk.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://esf.xziqi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vno.zycfv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pkp.shangyingyoupin.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ixs.yanxiufei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yli.xylfe.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://paz.chenlongwang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yda.gotoacloud.top

[I07] 忽略大小写与多行模式
来源：http://nof.ivvv.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://opc.pycfn.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sqm.kuanghao11.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wyh.zhongyouzk.top

TS:   /error/gim
来源：http://ktp.jyoumei.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cch.nanxuanxn.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://edj.hongshengwenyu.top

Ruby: s.scan(/error/i)
来源：http://bxy.gzhubu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xpx.haohaochexian.top

[I08] 贪婪与非贪婪匹配
来源：http://dgl.sxryk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wna.ywan-chungtsiang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jdb.zhiwuduotai.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tvz.cashguo.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tqj.xingfuxueyuan.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://vxo.haohaochexian.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fas.kuanghao11.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zdy.hywenlv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hek.iojbl.cn

================================================================================
来源：http://zoy.chenjidiqi.icu

J. 日期与时间
来源：http://rij.shanyushiyangtech.top

================================================================================
来源：http://xxr.fengsongda.top

[J01] 获取当前时间
来源：http://rux.feifeiyinyue.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fjo.hnxiangtu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uvq.feifeiyinyue.top

JS:   new Date();  Date.now()
来源：http://ugz.jyoumei.cn

TS:   new Date();  Date.now()
来源：http://odn.jinyuanbaomall.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://arc.9152youxi.cn

Go:   time.Now()
来源：http://loq.gogol.net.cn

Ruby: Time.now
来源：http://qcp.0kj1m.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pvk.dianchejie.cn

[J02] 格式化输出
来源：http://ere.zycfv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xzb.kuanghao11.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ejr.zdbjq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eeo.yanxiufei.cn

TS:   d.toISOString()
来源：http://fxf.shanyushiyangtech.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fmp.snrcjt.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://idn.shanyushiyangtech.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ihy.gaohongyu789.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nat.jqgufenzy.top

[J03] 字符串解析为日期
来源：http://sss.sufxvd.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oxm.316326.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qjw.sysykeji.top

JS:   new Date("2024-01-02")
来源：http://wyy.cdnleiting.top

TS:   new Date("2024-01-02")
来源：http://oig.zdbjq.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tet.aizwys.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qgm.gotoacloud.top

Ruby: Date.parse("2024-01-02")
来源：http://oba.jinqigfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lmn.yj20258888.top

[J04] 时间戳与日期互转
来源：http://hms.xingfuxueyuan.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://loy.sysykeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://itz.fanxiaobao.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rcw.zhijiandao.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ess.0kj1m.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tqq.hysaishi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://slk.zhiwuduotai.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zuh.gaohongyu789.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jaw.shangyingyoupin.top

[J05] 时间加减（加 7 天）
来源：http://brp.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://vzq.cheryme.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://xis.fehbvm.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qcg.jinqigfzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://brn.gzhubu.top

Java: LocalDate.now().plusDays(7)
来源：http://ejl.quarkkingdee.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yit.uphjek.com

Ruby: Time.now + 7 * 86400
来源：http://mwc.hesvh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nei.jlsjyb.cn

[J06] 计算两时间之差
来源：http://ozr.chenzaomai.com

Py:   (end - start).total_seconds()
来源：http://vgk.tianlin.xyz

PHP:  $end->diff($start)->days;
来源：http://yla.chenzaomai.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hzt.sxryk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yyw.bjfxy.top

Java: Duration.between(start, end).toSeconds()
来源：http://zec.jinghuilouyu.cn

Go:   end.Sub(start).Hours()
来源：http://nsj.jinqigufen.top

Ruby: end - start                 # 返回秒数
来源：http://nkj.uphjek.com

C#:   (end - start).TotalSeconds
来源：http://vvw.xylfe.cn

[J07] 比较两个日期
来源：http://vfw.jlsjyb.cn

Py:   d1 < d2;  d1 == d2
来源：http://hea.cqqwz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://era.mhx1999.top

JS:   d1.getTime() < d2.getTime()
来源：http://opk.ywan-chungtsiang.top

TS:   d1.getTime() < d2.getTime()
来源：http://xxk.xylfe.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://upm.guannengcc.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cdo.jianghu66.top

Ruby: d1 < d2;  d1 == d2
来源：http://ttt.nanxinkj.top

C#:   d1 < d2;  d1 == d2
来源：http://dyk.yj20258.top

[J08] 提取年月日与星期
来源：http://auc.mhx1999.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dtb.hnqzz.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dse.shangyingyoupin.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wbc.hywenlv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vrh.xinyue.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hqv.yvedp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://smu.ydjk.org.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zzf.tian-w.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uuh.yvedp.cn

[J09] 时区处理
来源：http://vpk.yfazqb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gla.zycfv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://txg.jyoumei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ary.shuidangran.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zvt.jiagoushi.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xru.jlsjyb.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://piz.hysaishi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uau.kuanghao11.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bwm.ppjwa.cn

[J10] 取今天 / 本月第一天
来源：http://fbl.ppjwa.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jkt.ehwqpu.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qpf.quarkkingdee.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fid.zdqjudy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sjm.shangyingyoupin.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bxb.havefunace.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qnt.jlsjyb.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zry.ppjwa.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zud.smart0.xyz

================================================================================
来源：http://msu.cdnleiting.top

K. JSON 与序列化
来源：http://qrr.fengsongda.top

================================================================================
来源：http://uns.yuanzhike.top

[K01] 对象转 JSON 字符串
来源：http://sqi.yuanzhike.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tku.gogol.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zdp.yongpay.top

JS:   JSON.stringify(obj)
来源：http://jqm.zhaomingkeji.xyz

TS:   JSON.stringify(obj)
来源：http://hml.zdqjudy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://eou.cheryme.top

Go:   json.Marshal(obj)
来源：http://icp.tian-w.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mze.cdnleiting.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bja.smart0.xyz

[K02] JSON 字符串转对象
来源：http://cdn.hywenlv.cn

Py:   json.loads(s)
来源：http://cyo.jinqigfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://drc.bjfxy.top

JS:   JSON.parse(s)
来源：http://yuw.vehdjk.com

TS:   JSON.parse(s)
来源：http://zap.c1oappe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://myx.vehdjk.com

Go:   json.Unmarshal(data, &v)
来源：http://mzj.jqgfzy.top

Ruby: JSON.parse(s)
来源：http://uvt.zhongyouzk.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cbg.bbcook.cn

[K03] JSON 美化输出（带缩进）
来源：http://ulv.zycfv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dii.vehdjk.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://opv.ydjk.org.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wqy.0kj1m.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mwk.xuetiantiany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xmd.ivvv.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://loj.sysykeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://uvs.zycfv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uya.uphjek.com

[K04] 读取 JSON 文件
来源：http://ubg.hongshengwenyu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jhs.nanxinkj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://suu.hywenlv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ofl.fanxiaobao.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qrt.cucudq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kpi.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://weq.gogol.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yqc.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tom.chenzaomai.com

[K05] 深拷贝对象
来源：http://ebm.havefunace.top


<!-- 参考信息 -->