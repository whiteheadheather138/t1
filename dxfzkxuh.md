代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://agv.aibaodan.cn

Ruby: obj.instance_variables
来源：http://oxt.guannengcc.top

C#:   // 用反射或 System.Text.Json
来源：http://mrt.nwbrower.top

================================================================================
来源：http://fxc.svipenyu.cn

H. 异常与错误处理
来源：http://yjo.vehdjk.com

================================================================================
来源：http://aog.pycfn.com

[H01] try / catch 基础
来源：http://cjm.yongpay.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://til.sysykeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yrv.ctjpmb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ugq.cdnleiting.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nsa.nanxinkj.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uxr.dashuyun.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lva.mhx1999.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xso.zhijiandao.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://szg.fzhhl.top

[H02] finally / ensure 收尾
来源：http://qjk.hongshengwenyu.top

Py:   try: f()⏎finally: cleanup()
来源：http://djd.shuidangran.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://guk.pengpengdd.cyou

JS:   try { f(); } finally { cleanup(); }
来源：http://xfn.zhoulong.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://vcn.yangfankeji.com

Java: try { f(); } finally { cleanup(); }
来源：http://pyi.zhiwuduotai.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://lvu.zhengqikj.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hab.daxiang520.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pjo.shuidangran.top

[H03] 主动抛出异常
来源：http://lnh.xuetiantiany.cn

Py:   raise ValueError("错误信息")
来源：http://pdn.yvedp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mvc.ybcxt.top

JS:   throw new Error("错误信息");
来源：http://cas.hnxiangtu.top

TS:   throw new Error("错误信息");
来源：http://giy.xingfuxueyuan.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://dyx.zhoulong.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uon.svipenyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ief.feifeiyinyue.top

C#:   throw new ArgumentException("错误信息");
来源：http://zsm.shanyushiyangtech.top

[H04] 自定义异常类型
来源：http://puq.pengpengdd.cyou

Py:   class MyError(Exception): pass
来源：http://fuh.c1oappe.top

PHP:  class MyError extends RuntimeException {}
来源：http://nwg.jyoumei.cn

JS:   class MyError extends Error {}
来源：http://ami.jqgufenzy.top

TS:   class MyError extends Error {}
来源：http://sjt.ivvv.top

Java: class MyException extends RuntimeException {}
来源：http://xhl.zycfv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mhx.andypj.xyz

Ruby: class MyError < StandardError; end
来源：http://uhp.sysykeji.top

C#:   class MyException : Exception {}
来源：http://lss.52xcode.cn

[H05] 捕获特定类型
来源：http://cib.smart0.xyz

Py:   except ValueError as e:
来源：http://ess.yj202588.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uki.mhx1999.top

JS:   if (e instanceof TypeError) {}
来源：http://nqx.tian-w.cn

TS:   if (e instanceof TypeError) {}
来源：http://tcq.sweek.top

Java: catch (IOException | SQLException e) {}
来源：http://kjl.fktsv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bek.sjlbkw.cn

Ruby: rescue ArgumentError => e
来源：http://lgm.zhaomingkeji.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ryx.ctjpmb.com

[H06] 可选值 / 空值安全访问
来源：http://zwp.chenlongwang.top

Py:   value = d.get("k") or default
来源：http://ylb.cashguo.top

PHP:  $v = $d["k"] ?? null;
来源：http://rzn.xziqi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fef.zdbjq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zim.tarul.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zwo.smart0.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://tsg.cashguo.top

Ruby: d&.dig(:a, :b)
来源：http://xze.jinqigfzy.top

C#:   obj?.A?.B ?? default
来源：http://zrl.gaohongyu789.top

[H07] 断言
来源：http://zls.shanyushiyangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://sej.tanke756.top

PHP:  assert($x > 0);
来源：http://cpp.52xcode.cn

JS:   console.assert(x > 0);
来源：http://vva.sufxvd.cn

TS:   console.assert(x > 0);
来源：http://rol.zhixingplan.top

Java: assert x > 0 : "必须为正";
来源：http://qfw.tarul.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ttc.tianlin.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://hbo.guowangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://cxw.ydzc1.top

[H08] 获取错误信息与堆栈
来源：http://tcr.svipenyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://ekf.chenzaomai.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nms.aizwys.cn

JS:   e.message;  e.stack
来源：http://mov.ivvv.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://uwn.yvedp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mbo.yuanzhike.top

Go:   err.Error()
来源：http://szo.bbcook.cn

Ruby: e.message;  e.backtrace
来源：http://onw.ydzc1.top

C#:   e.Message;  e.StackTrace
来源：http://yvn.9152youxi.cn

[H09] 带错误码的异常
来源：http://sun.fktsv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wao.yfazqb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://amr.ywan-chungtsiang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dxz.sjlbkw.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uak.xinyue.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zpt.yj202588.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oad.feifeiyinyue.top

Ruby: raise MyError.new("fail", 500)
来源：http://dwy.hnxiangtu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://mxo.zhoulong.xyz

[H10] 资源自动释放
来源：http://obn.vehdjk.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://olx.daria6918.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wpb.fzhhl.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://awp.pycfn.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://scs.316326.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tpa.jlsjyb.cn

Go:   defer f.Close()
来源：http://tho.zhoulong.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://btu.fktsv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nsx.hysaishi.cn

================================================================================
来源：http://xbr.jqgufenzy.top

I. 正则表达式
来源：http://lcn.gogol.net.cn

================================================================================
来源：http://gmn.zhiwuduotai.top

[I01] 判断是否匹配
来源：http://pkr.ppjwa.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ntl.hfpthk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yex.ctjpmb.com

JS:   /\d+/.test(s)
来源：http://oid.xuanzx.com

TS:   /\d+/.test(s)
来源：http://wve.yj20258.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uke.hammf.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://frz.sjlbkw.cn

Ruby: s.match?(/\d+/)
来源：http://pvf.epnwcf.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pxj.yj20258.top

[I02] 提取所有匹配
来源：http://avc.gogol.net.cn

Py:   re.findall(r"\d+", s)
来源：http://ucl.hnqzz.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zcc.tanke756.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mmu.andypj.xyz

TS:   s.match(/\d+/g)
来源：http://zlo.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ela.fehbvm.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wux.chenjidiqi.icu

Ruby: s.scan(/\d+/)
来源：http://adp.sjlbkw.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zeh.gotoacloud.top

[I03] 提取捕获分组
来源：http://idt.aibaodan.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cfo.ywan-chungtsiang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mea.daria6918.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xno.guannengcc.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lkf.chenjidiqi.icu

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mwg.sxryk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ydd.jyoumei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wfj.guannengcc.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fjr.yuxming.cn

[I04] 正则替换
来源：http://imq.nanxuanxn.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jzw.svipenyu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ehx.hcnkem.com

JS:   s.replace(/\d+/g, "#")
来源：http://usr.zhixingplan.top

TS:   s.replace(/\d+/g, "#")
来源：http://jxb.hysaishi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vyo.zhijiandao.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hom.hywenlv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://syw.tarul.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://swp.yuxming.cn

[I05] 按正则拆分
来源：http://kpi.hfpthk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mbm.fengsongda.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mbg.ydjk.org.cn

JS:   s.split(/\s*,\s*/)
来源：http://ivj.zhiwuduotai.top

TS:   s.split(/\s*,\s*/)
来源：http://zlq.dashuyun.cn

Java: s.split("\\s*,\\s*")
来源：http://cxa.nanxuanxn.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gea.pengpengdd.cyou

Ruby: s.split(/\s*,\s*/)
来源：http://kgd.fanxiaobao.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nki.cheryme.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ntd.chenjidiqi.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mov.xuanzx.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iwv.sjlbkw.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://umt.zycfv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tlh.bbcook.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mvo.xingfuxueyuan.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://puc.zhaomingkeji.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dwk.aizwys.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rnt.andypj.xyz

[I07] 忽略大小写与多行模式
来源：http://fwe.xylfe.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uls.c1oappe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xyb.zhijiandao.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eby.meibo888.top

TS:   /error/gim
来源：http://ulf.pycfn.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fvk.xinyue.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tgf.ydzc1.top

Ruby: s.scan(/error/i)
来源：http://iut.jiagoushi.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://szr.nwbrower.top

[I08] 贪婪与非贪婪匹配
来源：http://wrq.nwbrower.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jgi.dianchejie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fiu.nanxinkj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mcx.hcnkem.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qkg.zdqjudy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qgm.yvedp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zze.redwolf501.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zdr.c1oappe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tgc.aibaodan.cn

================================================================================
来源：http://acm.quarkkingdee.top

J. 日期与时间
来源：http://qfc.jqgufenzy.top

================================================================================
来源：http://sds.jlsjyb.cn

[J01] 获取当前时间
来源：http://wch.nanxuanxn.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jyi.nanxuanxn.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zgq.hywenlv.cn

JS:   new Date();  Date.now()
来源：http://miv.jiagoushi.top

TS:   new Date();  Date.now()
来源：http://wxu.sweek.top

Java: LocalDateTime.now();  Instant.now()
来源：http://zrd.chenjidiqi.icu

Go:   time.Now()
来源：http://szs.cdnleiting.top

Ruby: Time.now
来源：http://uev.gogol.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uaq.yongpay.top

[J02] 格式化输出
来源：http://bbe.sxryk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vku.redwolf501.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gev.sjlbkw.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://icp.ywan-chungtsiang.top

TS:   d.toISOString()
来源：http://wgg.jqgufenzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lsd.hfpthk.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nxf.snrcjt.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rrd.9152youxi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pyr.zhaomingkeji.xyz

[J03] 字符串解析为日期
来源：http://tty.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nit.nanxinkj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gmz.xuanzx.com

JS:   new Date("2024-01-02")
来源：http://gwc.haohaochexian.top

TS:   new Date("2024-01-02")
来源：http://spe.hnqzz.top

Java: LocalDate.parse("2024-01-02")
来源：http://uxb.hnxiangtu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jah.cheryme.top

Ruby: Date.parse("2024-01-02")
来源：http://gzm.fzhhl.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://soe.cashguo.top

[J04] 时间戳与日期互转
来源：http://iok.hnqzz.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://djh.yuanzhike.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://anx.feifeiyinyue.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zxq.shuidangran.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xuz.ydzc1.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ebn.9152youxi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vyl.sxryk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yrr.yangfankeji.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rvg.xylfe.cn

[J05] 时间加减（加 7 天）
来源：http://ntc.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://klu.aibaodan.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bdd.cucudq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://trk.mhx1999.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pkz.jqgfzy.top

Java: LocalDate.now().plusDays(7)
来源：http://vtj.hywenlv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zwk.jinyuanbaomall.cn

Ruby: Time.now + 7 * 86400
来源：http://kpu.shuidangran.top

C#:   DateTime.Now.AddDays(7)
来源：http://snd.feifeiyinyue.top

[J06] 计算两时间之差
来源：http://ubn.wangdashe.top

Py:   (end - start).total_seconds()
来源：http://pel.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://fnb.shanyushiyangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eqp.cheryme.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xmi.nanxinkj.top

Java: Duration.between(start, end).toSeconds()
来源：http://jkv.shanyushiyangkeji.top

Go:   end.Sub(start).Hours()
来源：http://wyj.nanxinkj.top

Ruby: end - start                 # 返回秒数
来源：http://ncm.chenlongwang.top

C#:   (end - start).TotalSeconds
来源：http://drl.sweek.top

[J07] 比较两个日期
来源：http://kzp.cashguo.top

Py:   d1 < d2;  d1 == d2
来源：http://ydh.iojbl.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jte.andypj.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://mra.jqgfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://rgg.ppjwa.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zpw.yuxming.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jxx.fktsv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pqx.yueranfly.top

C#:   d1 < d2;  d1 == d2
来源：http://tji.hcnkem.com

[J08] 提取年月日与星期
来源：http://cix.cdnleiting.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jlu.fanxiaobao.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hoh.shangyingyoupin.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://obt.bbcook.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oim.chenlongwang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bvt.guannengcc.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://eip.yvedp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zai.sysykeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ojg.tianlin.xyz

[J09] 时区处理
来源：http://fnj.zhaomingkeji.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tag.quarkkingdee.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wtn.aibaodan.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uao.yangfankeji.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jum.sufxvd.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aaq.shangyingyoupin.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rlj.sxryk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://npy.gogol.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://omw.vehdjk.com

[J10] 取今天 / 本月第一天
来源：http://lrq.sjlbkw.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://npw.ydjk.org.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ovs.hywenlv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ccj.quarkkingdee.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://klx.snrcjt.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ijj.sufxvd.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lnq.jinghuilouyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bpn.jlsjyb.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://aws.jqgufenzy.top

================================================================================
来源：http://ahp.meibo888.top

K. JSON 与序列化
来源：http://koc.jinyuanbaomall.cn

================================================================================
来源：http://nev.jqgufenzy.top

[K01] 对象转 JSON 字符串
来源：http://tdb.nanxinkj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yjr.yangfankeji.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ghs.xuanzx.com

JS:   JSON.stringify(obj)
来源：http://dsv.c1oappe.top

TS:   JSON.stringify(obj)
来源：http://jrs.jqgufenzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yur.gogol.net.cn

Go:   json.Marshal(obj)
来源：http://jdm.fehbvm.com

Ruby: obj.to_json                                     // require "json"
来源：http://dhv.jqgfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ize.bbcook.cn

[K02] JSON 字符串转对象
来源：http://xfv.svipenyu.cn

Py:   json.loads(s)
来源：http://utf.jinqigfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pki.ehwqpu.com

JS:   JSON.parse(s)
来源：http://qou.xziqi.cn

TS:   JSON.parse(s)
来源：http://eid.gaohongyu789.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://iou.yonumen.top

Go:   json.Unmarshal(data, &v)
来源：http://aru.yvedp.cn

Ruby: JSON.parse(s)
来源：http://mrl.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zwo.chenlongwang.top

[K03] JSON 美化输出（带缩进）
来源：http://ksf.fanxiaobao.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vau.hfpthk.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hkw.yangfankeji.com

JS:   JSON.stringify(obj, null, 2)
来源：http://zbn.ppjwa.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nxv.hcnkem.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ejm.shuidangran.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bec.hnxiangtu.top

Ruby: JSON.pretty_generate(obj)
来源：http://nkz.xuanzx.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yes.yangfankeji.com

[K04] 读取 JSON 文件
来源：http://wqm.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rdc.shzxlz.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gci.cucudq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mit.yongpay.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wia.yueranfly.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jlf.0kj1m.cn


<!-- 参考信息 -->