代发 wailian999

PHP:  get_object_vars($obj);
来源：http://htw.birdmap.top

JS:   Object.entries(obj)
来源：http://kke.fehbvm.com

TS:   Object.entries(obj)
来源：http://wee.xziqi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bvc.hfpthk.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wuo.sweek.top

Ruby: obj.instance_variables
来源：http://dyw.zdbjq.cn

C#:   // 用反射或 System.Text.Json
来源：http://lmv.hcnkem.com

================================================================================
来源：http://sql.zdqjudy.top

H. 异常与错误处理
来源：http://wsc.cqqwz.cn

================================================================================
来源：http://ksh.yueranfly.top

[H01] try / catch 基础
来源：http://lev.xylfe.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ayi.jinghuilouyu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yub.52xcode.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jdm.guannengcc.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ahp.bbcook.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cab.yangfankeji.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vsw.zhongyouzk.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qog.cucudq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fie.chenzaomai.com

[H02] finally / ensure 收尾
来源：http://xgi.yj20258888.top

Py:   try: f()⏎finally: cleanup()
来源：http://rhl.smart0.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://ehf.shanyushiyangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://aio.zhiwuduotai.top

TS:   try { f(); } finally { cleanup(); }
来源：http://cne.cucudq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rfv.sweek.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://txj.zhiwuduotai.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xuo.iojbl.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://owp.quarkkingdee.top

[H03] 主动抛出异常
来源：http://gon.fengsongda.top

Py:   raise ValueError("错误信息")
来源：http://ige.jinqigfzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kkw.smart0.xyz

JS:   throw new Error("错误信息");
来源：http://zgx.316326.xyz

TS:   throw new Error("错误信息");
来源：http://qln.kuanghao11.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wtx.sweek.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://inm.zhaomingkeji.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://bpg.meibo888.top

C#:   throw new ArgumentException("错误信息");
来源：http://kwb.guowangkeji.top

[H04] 自定义异常类型
来源：http://xkx.ywan-chungtsiang.top

Py:   class MyError(Exception): pass
来源：http://fsb.redwolf501.top

PHP:  class MyError extends RuntimeException {}
来源：http://hsj.dianchejie.cn

JS:   class MyError extends Error {}
来源：http://udi.yangfankeji.com

TS:   class MyError extends Error {}
来源：http://vzm.gotoacloud.top

Java: class MyException extends RuntimeException {}
来源：http://vuh.shanyushiyangkeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lte.xylfe.cn

Ruby: class MyError < StandardError; end
来源：http://onp.hnxiangtu.top

C#:   class MyException : Exception {}
来源：http://oxo.xingfuxueyuan.xyz

[H05] 捕获特定类型
来源：http://nty.jinqigufen.top

Py:   except ValueError as e:
来源：http://jwr.quarkkingdee.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rbo.meibo888.top

JS:   if (e instanceof TypeError) {}
来源：http://iwf.zdqjudy.top

TS:   if (e instanceof TypeError) {}
来源：http://dyy.sjlbkw.cn

Java: catch (IOException | SQLException e) {}
来源：http://hle.vehdjk.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hin.ivvv.top

Ruby: rescue ArgumentError => e
来源：http://fvx.yuxming.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gzi.zhongyouzk.top

[H06] 可选值 / 空值安全访问
来源：http://tip.smart0.xyz

Py:   value = d.get("k") or default
来源：http://yod.guowangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://evt.iojbl.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xnj.xylfe.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rkl.zhongyouzk.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rhv.quarkkingdee.top

Go:   if v, ok := m["k"]; ok { }
来源：http://puk.hammf.cn

Ruby: d&.dig(:a, :b)
来源：http://gje.gzhubu.top

C#:   obj?.A?.B ?? default
来源：http://xna.sjlbkw.cn

[H07] 断言
来源：http://yzu.zhengqikj.top

Py:   assert x > 0, "必须为正"
来源：http://zev.hywenlv.cn

PHP:  assert($x > 0);
来源：http://xoj.wangdashe.top

JS:   console.assert(x > 0);
来源：http://ymq.xylfe.cn

TS:   console.assert(x > 0);
来源：http://gfo.ybcxt.top

Java: assert x > 0 : "必须为正";
来源：http://dvk.jqgufenzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kmx.hysaishi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rma.shzxlz.cn

C#:   Debug.Assert(x > 0);
来源：http://wla.bjfxy.top

[H08] 获取错误信息与堆栈
来源：http://qss.gotoacloud.top

Py:   str(e);  traceback.format_exc()
来源：http://amo.c1oappe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fni.chenlongwang.top

JS:   e.message;  e.stack
来源：http://wad.yvedp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qif.cqqwz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ulv.ivvv.top

Go:   err.Error()
来源：http://orm.hammf.cn

Ruby: e.message;  e.backtrace
来源：http://hht.guowangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://qol.sysykeji.top

[H09] 带错误码的异常
来源：http://bhn.zhiwuduotai.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nnz.shangyingyoupin.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://eft.ctjpmb.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mst.cqqwz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vgk.guowangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hey.zdqjudy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lyu.ivvv.top

Ruby: raise MyError.new("fail", 500)
来源：http://czm.haohaochexian.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zsw.andypj.xyz

[H10] 资源自动释放
来源：http://fob.jinyuanbaomall.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gqg.hesvh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vut.nanxinkj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://noq.smart0.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tis.gogol.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wue.jqgfzy.top

Go:   defer f.Close()
来源：http://qvo.ybcxt.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vtk.wangdashe.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fud.zhixingplan.top

================================================================================
来源：http://lfy.wangdashe.top

I. 正则表达式
来源：http://aqx.wangshuangyany.cn

================================================================================
来源：http://mbn.shzxlz.cn

[I01] 判断是否匹配
来源：http://aog.hnqzz.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pcu.iojbl.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ssd.haohaochexian.top

JS:   /\d+/.test(s)
来源：http://cln.ehwqpu.com

TS:   /\d+/.test(s)
来源：http://scm.hcnkem.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mns.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lnz.sysykeji.top

Ruby: s.match?(/\d+/)
来源：http://sgp.hesvh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cbn.kuanghao11.cn

[I02] 提取所有匹配
来源：http://wde.yuxming.cn

Py:   re.findall(r"\d+", s)
来源：http://ulr.iojbl.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ejf.zhoulong.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zjc.0kj1m.cn

TS:   s.match(/\d+/g)
来源：http://tfl.yuxming.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uul.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qkg.gotoacloud.top

Ruby: s.scan(/\d+/)
来源：http://sqp.tarul.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rbp.gzhubu.top

[I03] 提取捕获分组
来源：http://vgf.ppjwa.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qke.jianghu66.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jda.yangfankeji.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://giy.tarul.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kjs.hammf.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uuw.cqqwz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yjm.tanke756.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hgo.yangfankeji.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dwq.hywenlv.cn

[I04] 正则替换
来源：http://zuo.jinyuanbaomall.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yhu.uphjek.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://een.fzhhl.top

JS:   s.replace(/\d+/g, "#")
来源：http://afw.316326.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://gpn.nanxinkj.top

Java: s.replaceAll("\\d+", "#")
来源：http://qst.jiagoushi.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lgi.hnqzz.top

Ruby: s.gsub(/\d+/, "#")
来源：http://phk.fzhhl.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sgo.ivvv.top

[I05] 按正则拆分
来源：http://ueg.zhiwuduotai.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ayg.nwbrower.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ool.zycfv.cn

JS:   s.split(/\s*,\s*/)
来源：http://vid.gzhubu.top

TS:   s.split(/\s*,\s*/)
来源：http://ntc.jqgufenzy.top

Java: s.split("\\s*,\\s*")
来源：http://peb.ydzc1.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yeu.xziqi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rtu.fehbvm.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://owm.haohaochexian.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yii.vqdsnc.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tei.tian-w.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pyl.chenzaomai.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qgp.andypj.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eyp.fanxiaobao.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hiw.yangfankeji.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fdm.hnxiangtu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eqr.feifeiyinyue.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sez.nanxinkj.top

[I07] 忽略大小写与多行模式
来源：http://cyi.shanyushiyangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://djq.jlsjyb.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ehr.cqqwz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dlv.aizwys.cn

TS:   /error/gim
来源：http://hqr.hnqzz.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ibm.shzxlz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qid.jinqigfzy.top

Ruby: s.scan(/error/i)
来源：http://mdj.c1oappe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://asi.smart0.xyz

[I08] 贪婪与非贪婪匹配
来源：http://lco.mhx1999.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mni.yuxming.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://knc.fengsongda.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ikb.316326.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gnx.ppjwa.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://eay.sweek.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bzt.xuanzx.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tkw.cdnleiting.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pls.gzhubu.top

================================================================================
来源：http://xdv.tian-w.cn

J. 日期与时间
来源：http://rxf.hfpthk.cn

================================================================================
来源：http://rge.jinqigfzy.top

[J01] 获取当前时间
来源：http://cto.shanyushiyangtech.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://tto.ybcxt.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zsm.sxryk.cn

JS:   new Date();  Date.now()
来源：http://sat.fzhhl.top

TS:   new Date();  Date.now()
来源：http://cqk.shzxlz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xzs.iojbl.cn

Go:   time.Now()
来源：http://ksw.meibo888.top

Ruby: Time.now
来源：http://msd.yvedp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hcr.uphjek.com

[J02] 格式化输出
来源：http://srf.daria6918.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://grr.ydzc1.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xmr.9152youxi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://soi.hesvh.cn

TS:   d.toISOString()
来源：http://ehs.aibaodan.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vzk.wangdashe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rrl.cqqwz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cuk.shanyushiyangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gpe.cdnleiting.top

[J03] 字符串解析为日期
来源：http://fdj.c1oappe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fka.jinqigufen.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bgg.shuidangran.top

JS:   new Date("2024-01-02")
来源：http://bjs.ppjwa.cn

TS:   new Date("2024-01-02")
来源：http://apv.hnxiangtu.top

Java: LocalDate.parse("2024-01-02")
来源：http://mxh.meibo888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sgk.hywenlv.cn

Ruby: Date.parse("2024-01-02")
来源：http://sko.yongpay.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jpv.daria6918.cn

[J04] 时间戳与日期互转
来源：http://ghe.gotoacloud.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wxt.ywan-chungtsiang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ysg.ehwqpu.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://djr.guowangkeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jey.jianghu66.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jmt.shanyushiyangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fte.sxryk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://voi.tarul.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zke.tanke756.top

[J05] 时间加减（加 7 天）
来源：http://hil.fengsongda.top

Py:   now + timedelta(days=7)
来源：http://wui.aizwys.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cet.yanxiufei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kxj.jiagoushi.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bjh.tanke756.top

Java: LocalDate.now().plusDays(7)
来源：http://unh.shzxlz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yoq.ehwqpu.com

Ruby: Time.now + 7 * 86400
来源：http://ezn.gzhubu.top

C#:   DateTime.Now.AddDays(7)
来源：http://vxv.fengsongda.top

[J06] 计算两时间之差
来源：http://jnq.jinqigfzy.top

Py:   (end - start).total_seconds()
来源：http://xmw.dianchejie.cn

PHP:  $end->diff($start)->days;
来源：http://yrt.fktsv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tqi.ybcxt.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ach.ctjpmb.com

Java: Duration.between(start, end).toSeconds()
来源：http://lut.guowangkeji.top

Go:   end.Sub(start).Hours()
来源：http://qxc.chenjidiqi.icu

Ruby: end - start                 # 返回秒数
来源：http://eme.snrcjt.cn

C#:   (end - start).TotalSeconds
来源：http://ysl.vehdjk.com

[J07] 比较两个日期
来源：http://btx.yueranfly.top

Py:   d1 < d2;  d1 == d2
来源：http://zgy.daria6918.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://usr.cheryme.top

JS:   d1.getTime() < d2.getTime()
来源：http://zjt.cheryme.top

TS:   d1.getTime() < d2.getTime()
来源：http://ucc.yuanzhike.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zme.vehdjk.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hwq.ybcxt.top

Ruby: d1 < d2;  d1 == d2
来源：http://ohk.bbcook.cn

C#:   d1 < d2;  d1 == d2
来源：http://dyp.yvedp.cn

[J08] 提取年月日与星期
来源：http://sgv.zhongyouzk.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hkr.bjfxy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kkx.shanyushiyangtech.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://clw.bbcook.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jsr.sjlbkw.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xff.hammf.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pld.ydzc1.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zlu.jinghuilouyu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fqb.ctjpmb.com

[J09] 时区处理
来源：http://yeb.jinyuanbaomall.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bgu.guowangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pqk.fktsv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gdj.cheryme.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fqo.shzxlz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mcx.cdnleiting.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oce.haohaochexian.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fww.shanyushiyangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qle.xuanzx.com

[J10] 取今天 / 本月第一天
来源：http://gvi.nwbrower.top

Py:   date.today();  date.today().replace(day=1)
来源：http://oug.quarkkingdee.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ecp.ctjpmb.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lsf.jlsjyb.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dcu.yvedp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bnq.shanyushiyangkeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lkv.xinyue.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://peu.zhixingplan.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ept.ivvv.top

================================================================================
来源：http://jdz.smart0.xyz

K. JSON 与序列化
来源：http://ybn.gzhubu.top

================================================================================
来源：http://pva.ybcxt.top

[K01] 对象转 JSON 字符串
来源：http://jpj.yuxming.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gpk.yonumen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zcq.jyoumei.cn

JS:   JSON.stringify(obj)
来源：http://tvf.sweek.top

TS:   JSON.stringify(obj)
来源：http://ofm.dianchejie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tds.sweek.top

Go:   json.Marshal(obj)
来源：http://gaf.yfazqb.com

Ruby: obj.to_json                                     // require "json"
来源：http://zcj.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj)
来源：http://yri.andypj.xyz

[K02] JSON 字符串转对象
来源：http://xhc.sjlbkw.cn

Py:   json.loads(s)
来源：http://fbn.jqgfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wzp.quarkkingdee.top

JS:   JSON.parse(s)
来源：http://cub.wangshuangyany.cn

TS:   JSON.parse(s)
来源：http://wwi.shanyushiyangtech.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bmt.hnxiangtu.top

Go:   json.Unmarshal(data, &v)
来源：http://kyb.hnxiangtu.top

Ruby: JSON.parse(s)
来源：http://ygr.birdmap.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mjt.sjlbkw.cn

[K03] JSON 美化输出（带缩进）
来源：http://dnx.fehbvm.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dii.andypj.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vhy.sufxvd.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rad.shanyushiyangkeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mgt.zhoulong.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cgg.yfazqb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qsv.hnqzz.top

Ruby: JSON.pretty_generate(obj)
来源：http://vdk.meibo888.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vrm.epnwcf.com

[K04] 读取 JSON 文件
来源：http://ssd.xziqi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gjl.jqgfzy.top


<!-- 参考信息 -->