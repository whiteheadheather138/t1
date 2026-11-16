代发 wailian999

PHP:  get_object_vars($obj);
来源：http://ubk.ivvv.top

JS:   Object.entries(obj)
来源：http://evw.jinqigufen.top

TS:   Object.entries(obj)
来源：http://wgg.snrcjt.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://arh.ppjwa.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cgy.tanke756.top

Ruby: obj.instance_variables
来源：http://zzp.jiagoushi.top

C#:   // 用反射或 System.Text.Json
来源：http://xqe.yanxiufei.cn

================================================================================
来源：http://ndu.jinqigfzy.top

H. 异常与错误处理
来源：http://yfg.xinyue.icu

================================================================================
来源：http://bpp.kuanghao11.cn

[H01] try / catch 基础
来源：http://wih.haohaochexian.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://das.c1oappe.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ndb.hfpthk.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://swq.gotoacloud.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rnj.zhengqikj.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yxn.jyoumei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oek.fengsongda.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qhn.daxiang520.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ubw.epnwcf.com

[H02] finally / ensure 收尾
来源：http://pxx.yj20258888.top

Py:   try: f()⏎finally: cleanup()
来源：http://ldt.yuxming.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dmg.chenlongwang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rtw.tarul.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fsl.hfpthk.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jla.jiagoushi.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xow.yonumen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hvg.hcnkem.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://vtx.fehbvm.com

[H03] 主动抛出异常
来源：http://tgl.daria6918.cn

Py:   raise ValueError("错误信息")
来源：http://scv.shuidangran.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cum.sxryk.cn

JS:   throw new Error("错误信息");
来源：http://kqq.hfpthk.cn

TS:   throw new Error("错误信息");
来源：http://sxj.wangshuangyany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cgp.yangfankeji.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ukm.jianghu66.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lzr.nwbrower.top

C#:   throw new ArgumentException("错误信息");
来源：http://mqm.dashuyun.cn

[H04] 自定义异常类型
来源：http://ywf.ehwqpu.com

Py:   class MyError(Exception): pass
来源：http://dii.yanxiufei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rhz.jqgufenzy.top

JS:   class MyError extends Error {}
来源：http://shh.jiagoushi.top

TS:   class MyError extends Error {}
来源：http://hmz.birdmap.top

Java: class MyException extends RuntimeException {}
来源：http://tgm.xinyue.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zpr.xinyue.icu

Ruby: class MyError < StandardError; end
来源：http://ibk.gotoacloud.top

C#:   class MyException : Exception {}
来源：http://fux.feifeiyinyue.top

[H05] 捕获特定类型
来源：http://gsy.jyoumei.cn

Py:   except ValueError as e:
来源：http://smi.bbcook.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rbg.redwolf501.top

JS:   if (e instanceof TypeError) {}
来源：http://atw.zhijiandao.cn

TS:   if (e instanceof TypeError) {}
来源：http://xee.jiagoushi.top

Java: catch (IOException | SQLException e) {}
来源：http://lao.smart0.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://myr.xziqi.cn

Ruby: rescue ArgumentError => e
来源：http://lci.cashguo.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zjl.xinyue.icu

[H06] 可选值 / 空值安全访问
来源：http://hxi.zhixingplan.top

Py:   value = d.get("k") or default
来源：http://tbr.ywan-chungtsiang.top

PHP:  $v = $d["k"] ?? null;
来源：http://bml.fengsongda.top

JS:   obj?.a?.b;  d ?? default
来源：http://jai.chenlongwang.top

TS:   obj?.a?.b;  d ?? default
来源：http://csv.quarkkingdee.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://txw.hesvh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ydt.zhijiandao.cn

Ruby: d&.dig(:a, :b)
来源：http://gux.vehdjk.com

C#:   obj?.A?.B ?? default
来源：http://hcu.fanxiaobao.xyz

[H07] 断言
来源：http://bvr.hnxiangtu.top

Py:   assert x > 0, "必须为正"
来源：http://ldd.yongpay.top

PHP:  assert($x > 0);
来源：http://thj.zhaomingkeji.xyz

JS:   console.assert(x > 0);
来源：http://lpx.quarkkingdee.top

TS:   console.assert(x > 0);
来源：http://lvz.hammf.cn

Java: assert x > 0 : "必须为正";
来源：http://frb.daxiang520.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ryr.vehdjk.com

Ruby: raise "必须为正" unless x > 0
来源：http://kzn.xylfe.cn

C#:   Debug.Assert(x > 0);
来源：http://civ.xinyue.icu

[H08] 获取错误信息与堆栈
来源：http://cxo.daxiang520.top

Py:   str(e);  traceback.format_exc()
来源：http://jia.0kj1m.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bkp.yvedp.cn

JS:   e.message;  e.stack
来源：http://lev.jinqigufen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://gmj.gaohongyu789.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gzk.shuidangran.top

Go:   err.Error()
来源：http://ufo.xuetiantiany.cn

Ruby: e.message;  e.backtrace
来源：http://eou.fzhhl.top

C#:   e.Message;  e.StackTrace
来源：http://gbk.fanxiaobao.xyz

[H09] 带错误码的异常
来源：http://ovf.jinqigfzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nmv.xuanzx.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://cur.hfpthk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://npq.jinghuilouyu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bvv.bjfxy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nwq.sxryk.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yvr.yfazqb.com

Ruby: raise MyError.new("fail", 500)
来源：http://opf.nwbrower.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vvq.mhx1999.top

[H10] 资源自动释放
来源：http://wog.nanxuanxn.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://tys.xuanzx.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ouy.chenlongwang.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://plh.quarkkingdee.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yde.jyoumei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nfe.xuetiantiany.cn

Go:   defer f.Close()
来源：http://rhu.daria6918.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dwo.wangdashe.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pxh.dashuyun.cn

================================================================================
来源：http://oga.zhoulong.xyz

I. 正则表达式
来源：http://ohz.shanyushiyangkeji.top

================================================================================
来源：http://lzf.chenlongwang.top

[I01] 判断是否匹配
来源：http://aaw.fanxiaobao.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dtr.epnwcf.com

PHP:  preg_match('/\d+/', $s);
来源：http://wsa.ivvv.top

JS:   /\d+/.test(s)
来源：http://xpt.jiagoushi.top

TS:   /\d+/.test(s)
来源：http://ork.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eoe.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fku.fzhhl.top

Ruby: s.match?(/\d+/)
来源：http://ycf.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://aaj.ywan-chungtsiang.top

[I02] 提取所有匹配
来源：http://wwy.jinghuilouyu.cn

Py:   re.findall(r"\d+", s)
来源：http://aid.daria6918.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wlv.fengsongda.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jog.ivvv.top

TS:   s.match(/\d+/g)
来源：http://uzq.sweek.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cqk.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ezb.zhengqikj.top

Ruby: s.scan(/\d+/)
来源：http://vla.guowangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zdo.smart0.xyz

[I03] 提取捕获分组
来源：http://uzu.sxryk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zxd.nanxuanxn.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xdm.zhaomingkeji.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hfz.chenlongwang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hzq.zycfv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zor.yj20258.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bqp.316326.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://khd.fanxiaobao.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ktx.ybcxt.top

[I04] 正则替换
来源：http://cql.andypj.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://kse.quarkkingdee.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qnp.tianlin.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://uai.daria6918.cn

TS:   s.replace(/\d+/g, "#")
来源：http://igw.zdqjudy.top

Java: s.replaceAll("\\d+", "#")
来源：http://fcy.yj202588.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xsa.shuidangran.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xgn.epnwcf.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kev.sysykeji.top

[I05] 按正则拆分
来源：http://tmu.ydjk.org.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zot.yj202588.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uuk.shuidangran.top

JS:   s.split(/\s*,\s*/)
来源：http://upp.vehdjk.com

TS:   s.split(/\s*,\s*/)
来源：http://xsk.xuetiantiany.cn

Java: s.split("\\s*,\\s*")
来源：http://xsq.tian-w.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nkh.fengsongda.top

Ruby: s.split(/\s*,\s*/)
来源：http://lhp.iojbl.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jhd.dashuyun.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://crk.jianghu66.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jro.gogol.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lyl.hesvh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hzb.havefunace.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pwj.ehwqpu.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qkt.yvedp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://snm.tianlin.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lwy.nwbrower.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eif.hcnkem.com

[I07] 忽略大小写与多行模式
来源：http://gie.zhiwuduotai.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sne.yuanzhike.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://czx.redwolf501.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://smi.dianchejie.cn

TS:   /error/gim
来源：http://bfe.guowangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://eje.hongshengwenyu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://avu.aizwys.cn

Ruby: s.scan(/error/i)
来源：http://oey.hnqzz.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://muk.shzxlz.cn

[I08] 贪婪与非贪婪匹配
来源：http://cnp.gzhubu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dlb.jiagoushi.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wcw.c1oappe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zvl.zhaomingkeji.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sno.ehwqpu.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://tfl.redwolf501.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://osu.zhengqikj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ksy.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jir.jinqigfzy.top

================================================================================
来源：http://rhj.zhaomingkeji.xyz

J. 日期与时间
来源：http://whk.jlsjyb.cn

================================================================================
来源：http://gat.nanxuanxn.top

[J01] 获取当前时间
来源：http://ygk.sjlbkw.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lnu.andypj.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hph.zdbjq.cn

JS:   new Date();  Date.now()
来源：http://kyz.tian-w.cn

TS:   new Date();  Date.now()
来源：http://ptl.hysaishi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rzv.nwbrower.top

Go:   time.Now()
来源：http://umx.yuxming.cn

Ruby: Time.now
来源：http://evt.sysykeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yco.tarul.cn

[J02] 格式化输出
来源：http://wid.haohaochexian.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dui.haohaochexian.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fru.zhengqikj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cgn.jinqigfzy.top

TS:   d.toISOString()
来源：http://odi.ydjk.org.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mqd.iojbl.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hex.sysykeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bhb.cdnleiting.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yfl.sysykeji.top

[J03] 字符串解析为日期
来源：http://tut.316326.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kke.jinyuanbaomall.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hgm.jiagoushi.top

JS:   new Date("2024-01-02")
来源：http://nxh.jinqigfzy.top

TS:   new Date("2024-01-02")
来源：http://zws.mhx1999.top

Java: LocalDate.parse("2024-01-02")
来源：http://wui.jyoumei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fyo.iojbl.cn

Ruby: Date.parse("2024-01-02")
来源：http://atg.nanxinkj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://emw.daria6918.cn

[J04] 时间戳与日期互转
来源：http://woj.hesvh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cbj.fehbvm.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fqy.bjfxy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jqn.fengsongda.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zyb.birdmap.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aya.cheryme.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vow.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ymz.wangshuangyany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ufp.zycfv.cn

[J05] 时间加减（加 7 天）
来源：http://ffa.cqqwz.cn

Py:   now + timedelta(days=7)
来源：http://zfr.tarul.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hil.bbcook.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ooh.snrcjt.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dsm.0kj1m.cn

Java: LocalDate.now().plusDays(7)
来源：http://ptc.xylfe.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jkl.havefunace.top

Ruby: Time.now + 7 * 86400
来源：http://shs.zhixingplan.top

C#:   DateTime.Now.AddDays(7)
来源：http://avp.hcnkem.com

[J06] 计算两时间之差
来源：http://ocu.cucudq.cn

Py:   (end - start).total_seconds()
来源：http://yig.yonumen.top

PHP:  $end->diff($start)->days;
来源：http://cnf.bjfxy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sqb.bjfxy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cpo.ivvv.top

Java: Duration.between(start, end).toSeconds()
来源：http://ouz.pycfn.com

Go:   end.Sub(start).Hours()
来源：http://hhl.nwbrower.top

Ruby: end - start                 # 返回秒数
来源：http://lyv.zhaomingkeji.xyz

C#:   (end - start).TotalSeconds
来源：http://brw.cashguo.top

[J07] 比较两个日期
来源：http://dmu.kuanghao11.cn

Py:   d1 < d2;  d1 == d2
来源：http://tns.zycfv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rcs.yuanzhike.top

JS:   d1.getTime() < d2.getTime()
来源：http://jav.daxiang520.top

TS:   d1.getTime() < d2.getTime()
来源：http://hct.ydzc1.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kwt.guannengcc.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ggy.cucudq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sjk.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://twv.wangshuangyany.cn

[J08] 提取年月日与星期
来源：http://pce.mhx1999.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kvx.shanyushiyangtech.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tyz.zhiwuduotai.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mfb.xuetiantiany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://clv.xylfe.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aob.mhx1999.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gtt.shzxlz.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lfh.chenjidiqi.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rte.zhongyouzk.top

[J09] 时区处理
来源：http://hnd.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tab.snrcjt.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lrb.tian-w.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dab.jlsjyb.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nxg.tanke756.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://awk.ydjk.org.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dbu.xuetiantiany.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zzu.jqgufenzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bnb.jinyuanbaomall.cn

[J10] 取今天 / 本月第一天
来源：http://hig.hysaishi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qmu.birdmap.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eau.jqgfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bnv.ivvv.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://njr.redwolf501.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zhe.zhixingplan.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://iiw.daxiang520.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xwr.sjlbkw.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zgp.jinqigufen.top

================================================================================
来源：http://ylm.pengpengdd.cyou

K. JSON 与序列化
来源：http://czp.hnxiangtu.top

================================================================================
来源：http://jqg.bbcook.cn

[K01] 对象转 JSON 字符串
来源：http://gdr.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jor.ivvv.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gnq.cqqwz.cn

JS:   JSON.stringify(obj)
来源：http://bnu.ydjk.org.cn

TS:   JSON.stringify(obj)
来源：http://pvb.tarul.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://owz.tanke756.top

Go:   json.Marshal(obj)
来源：http://mhj.wangdashe.top

Ruby: obj.to_json                                     // require "json"
来源：http://lqg.haohaochexian.top

C#:   JsonSerializer.Serialize(obj)
来源：http://api.hysaishi.cn

[K02] JSON 字符串转对象
来源：http://rpt.aizwys.cn

Py:   json.loads(s)
来源：http://uit.bjfxy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xrl.xinyue.icu

JS:   JSON.parse(s)
来源：http://eaj.gaohongyu789.top

TS:   JSON.parse(s)
来源：http://ssb.mhx1999.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jov.sysykeji.top

Go:   json.Unmarshal(data, &v)
来源：http://psc.aibaodan.cn

Ruby: JSON.parse(s)
来源：http://trl.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fat.chenzaomai.com

[K03] JSON 美化输出（带缩进）
来源：http://rfh.cdnleiting.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://smf.hongshengwenyu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hvw.gotoacloud.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pfr.ybcxt.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ddm.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oet.yueranfly.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fva.quarkkingdee.top

Ruby: JSON.pretty_generate(obj)
来源：http://csi.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kxl.wangdashe.top

[K04] 读取 JSON 文件
来源：http://imi.shangyingyoupin.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://psx.gaohongyu789.top


<!-- 参考信息 -->