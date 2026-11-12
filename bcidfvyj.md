代发 wailian999

PHP:  get_object_vars($obj);
来源：http://mbo.chenzaomai.com

JS:   Object.entries(obj)
来源：http://riu.jinqigufen.top

TS:   Object.entries(obj)
来源：http://wve.0kj1m.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://noo.chenjidiqi.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://duu.jinghuilouyu.cn

Ruby: obj.instance_variables
来源：http://wjq.xuanzx.com

C#:   // 用反射或 System.Text.Json
来源：http://eos.wangdashe.top

================================================================================
来源：http://rln.hcnkem.com

H. 异常与错误处理
来源：http://spc.ctjpmb.com

================================================================================
来源：http://sjr.jiagoushi.top

[H01] try / catch 基础
来源：http://hsp.tarul.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uat.hongshengwenyu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://quz.pengpengdd.cyou

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cck.ppjwa.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://urm.aibaodan.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pmf.chenlongwang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hyp.havefunace.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ufc.chenlongwang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uyi.haohaochexian.top

[H02] finally / ensure 收尾
来源：http://erk.ctjpmb.com

Py:   try: f()⏎finally: cleanup()
来源：http://alu.yanxiufei.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zpw.tarul.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xpz.zycfv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fqs.cqqwz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bry.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://okn.svipenyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hbm.xinyue.icu

C#:   try { F(); } finally { Cleanup(); }
来源：http://akq.snrcjt.cn

[H03] 主动抛出异常
来源：http://krb.jianghu66.top

Py:   raise ValueError("错误信息")
来源：http://kmx.chenzaomai.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://prl.zhongyouzk.top

JS:   throw new Error("错误信息");
来源：http://dpj.hnqzz.top

TS:   throw new Error("错误信息");
来源：http://wav.guannengcc.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nfn.pengpengdd.cyou

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gze.vqdsnc.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://atq.zhiwuduotai.top

C#:   throw new ArgumentException("错误信息");
来源：http://hcb.c1oappe.top

[H04] 自定义异常类型
来源：http://nyn.quarkkingdee.top

Py:   class MyError(Exception): pass
来源：http://btl.haohaochexian.top

PHP:  class MyError extends RuntimeException {}
来源：http://toi.zdqjudy.top

JS:   class MyError extends Error {}
来源：http://gsu.shuidangran.top

TS:   class MyError extends Error {}
来源：http://ios.zdqjudy.top

Java: class MyException extends RuntimeException {}
来源：http://dkq.hnxiangtu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://izd.gogol.net.cn

Ruby: class MyError < StandardError; end
来源：http://sod.fanxiaobao.xyz

C#:   class MyException : Exception {}
来源：http://lej.fengsongda.top

[H05] 捕获特定类型
来源：http://eta.jyoumei.cn

Py:   except ValueError as e:
来源：http://wiz.52xcode.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://krh.sjlbkw.cn

JS:   if (e instanceof TypeError) {}
来源：http://hos.hnqzz.top

TS:   if (e instanceof TypeError) {}
来源：http://dpm.zhijiandao.cn

Java: catch (IOException | SQLException e) {}
来源：http://tdd.fehbvm.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ndo.shanyushiyangtech.top

Ruby: rescue ArgumentError => e
来源：http://qct.gotoacloud.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://stn.aizwys.cn

[H06] 可选值 / 空值安全访问
来源：http://xlq.yangfankeji.com

Py:   value = d.get("k") or default
来源：http://ztq.pycfn.com

PHP:  $v = $d["k"] ?? null;
来源：http://uiv.yj202588.top

JS:   obj?.a?.b;  d ?? default
来源：http://nuo.smart0.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://jsi.snrcjt.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wef.c1oappe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://isi.ywan-chungtsiang.top

Ruby: d&.dig(:a, :b)
来源：http://noe.tian-w.cn

C#:   obj?.A?.B ?? default
来源：http://pgz.tian-w.cn

[H07] 断言
来源：http://cpr.tanke756.top

Py:   assert x > 0, "必须为正"
来源：http://vyx.shzxlz.cn

PHP:  assert($x > 0);
来源：http://vao.wangdashe.top

JS:   console.assert(x > 0);
来源：http://dxt.tian-w.cn

TS:   console.assert(x > 0);
来源：http://jgf.zhongyouzk.top

Java: assert x > 0 : "必须为正";
来源：http://wpg.ivvv.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vpt.fehbvm.com

Ruby: raise "必须为正" unless x > 0
来源：http://mfm.jiagoushi.top

C#:   Debug.Assert(x > 0);
来源：http://bwb.shangyingyoupin.top

[H08] 获取错误信息与堆栈
来源：http://doi.sweek.top

Py:   str(e);  traceback.format_exc()
来源：http://odm.redwolf501.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oyc.cashguo.top

JS:   e.message;  e.stack
来源：http://slv.yanxiufei.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nfw.gogol.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://biz.mhx1999.top

Go:   err.Error()
来源：http://yvf.zdbjq.cn

Ruby: e.message;  e.backtrace
来源：http://ukx.jlsjyb.cn

C#:   e.Message;  e.StackTrace
来源：http://fjb.nanxinkj.top

[H09] 带错误码的异常
来源：http://tmu.meibo888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bdo.tanke756.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://zwp.dianchejie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gfz.nanxuanxn.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://izr.epnwcf.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://knv.xuetiantiany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lmg.snrcjt.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bfy.shuidangran.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ggq.yfazqb.com

[H10] 资源自动释放
来源：http://idw.jinghuilouyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://oum.316326.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qpf.uphjek.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ctt.cucudq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://alv.tarul.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://joz.yj202588.top

Go:   defer f.Close()
来源：http://rma.gotoacloud.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xlc.nanxinkj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qcy.jinqigfzy.top

================================================================================
来源：http://wqv.xziqi.cn

I. 正则表达式
来源：http://qci.nanxuanxn.top

================================================================================
来源：http://zdy.zycfv.cn

[I01] 判断是否匹配
来源：http://nes.yanxiufei.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tty.sysykeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://ayd.gotoacloud.top

JS:   /\d+/.test(s)
来源：http://icy.chenlongwang.top

TS:   /\d+/.test(s)
来源：http://hpr.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://idi.hnqzz.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uqj.yangfankeji.com

Ruby: s.match?(/\d+/)
来源：http://apn.pengpengdd.cyou

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ahk.yj20258.top

[I02] 提取所有匹配
来源：http://yft.hesvh.cn

Py:   re.findall(r"\d+", s)
来源：http://gwn.guowangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ygl.snrcjt.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://btz.zycfv.cn

TS:   s.match(/\d+/g)
来源：http://nxc.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ick.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://avr.birdmap.top

Ruby: s.scan(/\d+/)
来源：http://qni.chenzaomai.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wwp.smart0.xyz

[I03] 提取捕获分组
来源：http://rij.zhongyouzk.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kck.feifeiyinyue.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://eew.kuanghao11.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rtx.sysykeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://but.zdbjq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eni.yj20258.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kbv.iojbl.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hfk.zhijiandao.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jwz.epnwcf.com

[I04] 正则替换
来源：http://gll.snrcjt.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://znw.mhx1999.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wes.sxryk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kds.daxiang520.top

TS:   s.replace(/\d+/g, "#")
来源：http://bbu.sufxvd.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cvz.daria6918.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://utu.pycfn.com

Ruby: s.gsub(/\d+/, "#")
来源：http://nwn.316326.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yqr.xziqi.cn

[I05] 按正则拆分
来源：http://xbb.mhx1999.top

Py:   re.split(r"\s*,\s*", s)
来源：http://dkk.chenlongwang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xyr.wangshuangyany.cn

JS:   s.split(/\s*,\s*/)
来源：http://swe.shanyushiyangtech.top

TS:   s.split(/\s*,\s*/)
来源：http://xcj.snrcjt.cn

Java: s.split("\\s*,\\s*")
来源：http://cbn.sxryk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jua.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://clt.nanxinkj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xwx.yongpay.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://evp.0kj1m.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uif.chenjidiqi.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bej.hcnkem.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jad.hongshengwenyu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ajp.yuxming.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qbb.chenlongwang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dth.haohaochexian.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lhu.tanke756.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vkg.fengsongda.top

[I07] 忽略大小写与多行模式
来源：http://wzy.zhijiandao.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://put.gogol.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rco.jyoumei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mez.ywan-chungtsiang.top

TS:   /error/gim
来源：http://hue.yj20258888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mja.yanxiufei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ief.zhixingplan.top

Ruby: s.scan(/error/i)
来源：http://khg.chenzaomai.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hba.vqdsnc.cn

[I08] 贪婪与非贪婪匹配
来源：http://fel.birdmap.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lsh.daria6918.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://spf.yj20258888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gsn.cheryme.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://btv.guowangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ibm.shuidangran.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ciy.quarkkingdee.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gdw.hnqzz.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pox.yangfankeji.com

================================================================================
来源：http://mbz.xylfe.cn

J. 日期与时间
来源：http://qwq.jqgfzy.top

================================================================================
来源：http://fuy.iojbl.cn

[J01] 获取当前时间
来源：http://fdt.epnwcf.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://vjr.jlsjyb.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ckp.birdmap.top

JS:   new Date();  Date.now()
来源：http://irq.tanke756.top

TS:   new Date();  Date.now()
来源：http://qml.52xcode.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ojf.shanyushiyangtech.top

Go:   time.Now()
来源：http://eok.birdmap.top

Ruby: Time.now
来源：http://qvl.yj20258.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mul.xuetiantiany.cn

[J02] 格式化输出
来源：http://zcl.hesvh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vxf.0kj1m.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zwz.quarkkingdee.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dzq.xziqi.cn

TS:   d.toISOString()
来源：http://grd.zdbjq.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uqa.shanyushiyangtech.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://myw.sjlbkw.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xle.nanxuanxn.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://moa.ywan-chungtsiang.top

[J03] 字符串解析为日期
来源：http://swj.ydzc1.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ibr.birdmap.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kef.yj20258888.top

JS:   new Date("2024-01-02")
来源：http://jic.birdmap.top

TS:   new Date("2024-01-02")
来源：http://uue.guowangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://yxh.fehbvm.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bbe.ydzc1.top

Ruby: Date.parse("2024-01-02")
来源：http://nud.jinqigufen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hsx.fanxiaobao.xyz

[J04] 时间戳与日期互转
来源：http://zrc.yueranfly.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bdu.xziqi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lle.feifeiyinyue.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ilz.guowangkeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jtr.jinghuilouyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oli.zhengqikj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lhb.zhiwuduotai.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sxc.yuanzhike.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tbs.chenjidiqi.icu

[J05] 时间加减（加 7 天）
来源：http://djn.kuanghao11.cn

Py:   now + timedelta(days=7)
来源：http://ekl.xylfe.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://spd.tian-w.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uwv.dianchejie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tkv.guowangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://qrv.pycfn.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hsu.yvedp.cn

Ruby: Time.now + 7 * 86400
来源：http://fka.hnqzz.top

C#:   DateTime.Now.AddDays(7)
来源：http://iff.cheryme.top

[J06] 计算两时间之差
来源：http://unf.svipenyu.cn

Py:   (end - start).total_seconds()
来源：http://gfg.ehwqpu.com

PHP:  $end->diff($start)->days;
来源：http://qkh.ydzc1.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vjk.hnxiangtu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hvq.fzhhl.top

Java: Duration.between(start, end).toSeconds()
来源：http://sji.pycfn.com

Go:   end.Sub(start).Hours()
来源：http://zgm.nwbrower.top

Ruby: end - start                 # 返回秒数
来源：http://knd.ydzc1.top

C#:   (end - start).TotalSeconds
来源：http://szc.andypj.xyz

[J07] 比较两个日期
来源：http://tfh.haohaochexian.top

Py:   d1 < d2;  d1 == d2
来源：http://vyh.jinyuanbaomall.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lnm.ywan-chungtsiang.top

JS:   d1.getTime() < d2.getTime()
来源：http://ffp.zhongyouzk.top

TS:   d1.getTime() < d2.getTime()
来源：http://wmd.fehbvm.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lxt.sjlbkw.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uzm.quarkkingdee.top

Ruby: d1 < d2;  d1 == d2
来源：http://jbt.sysykeji.top

C#:   d1 < d2;  d1 == d2
来源：http://kch.xziqi.cn

[J08] 提取年月日与星期
来源：http://ezd.ctjpmb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wkr.ctjpmb.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jhj.jqgufenzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ouv.ywan-chungtsiang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jky.hfpthk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pup.ehwqpu.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ika.aibaodan.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jiw.cucudq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wnd.zycfv.cn

[J09] 时区处理
来源：http://qgm.zhiwuduotai.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jkw.zhixingplan.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sjv.ppjwa.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mrx.jinqigfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sbg.chenlongwang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://psx.dashuyun.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nwe.birdmap.top

Ruby: Time.now.getlocal("+08:00")
来源：http://oss.tarul.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qnl.redwolf501.top

[J10] 取今天 / 本月第一天
来源：http://vsy.xziqi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://occ.zdbjq.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qeg.gogol.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vog.dianchejie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qpq.yuanzhike.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zin.gotoacloud.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uti.jinqigufen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dfa.xuetiantiany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ffp.tianlin.xyz

================================================================================
来源：http://yjb.jinghuilouyu.cn

K. JSON 与序列化
来源：http://wvp.tian-w.cn

================================================================================
来源：http://ltn.shanyushiyangkeji.top

[K01] 对象转 JSON 字符串
来源：http://vsc.xuetiantiany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jpv.ehwqpu.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://euh.zycfv.cn

JS:   JSON.stringify(obj)
来源：http://aru.jinghuilouyu.cn

TS:   JSON.stringify(obj)
来源：http://kdf.cqqwz.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kqd.shangyingyoupin.top

Go:   json.Marshal(obj)
来源：http://fqr.yuanzhike.top

Ruby: obj.to_json                                     // require "json"
来源：http://cyf.birdmap.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cip.bjfxy.top

[K02] JSON 字符串转对象
来源：http://yol.vehdjk.com

Py:   json.loads(s)
来源：http://qid.zhongyouzk.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ods.sysykeji.top

JS:   JSON.parse(s)
来源：http://wip.zhoulong.xyz

TS:   JSON.parse(s)
来源：http://vzt.ywan-chungtsiang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jmg.nwbrower.top

Go:   json.Unmarshal(data, &v)
来源：http://dmk.hnqzz.top

Ruby: JSON.parse(s)
来源：http://nta.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qyj.zhijiandao.cn

[K03] JSON 美化输出（带缩进）
来源：http://rpj.wangdashe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vtb.shangyingyoupin.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hgd.epnwcf.com

JS:   JSON.stringify(obj, null, 2)
来源：http://aaa.fzhhl.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xms.ehwqpu.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tet.jinyuanbaomall.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://isd.zdbjq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://stc.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mnh.ydjk.org.cn

[K04] 读取 JSON 文件
来源：http://feb.cheryme.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rng.redwolf501.top


<!-- 参考信息 -->