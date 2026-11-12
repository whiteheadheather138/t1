代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nhd.ehwqpu.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yvj.ivvv.top

Java: enum Color { RED, GREEN }
来源：http://cnh.nanxinkj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xhw.9152youxi.cn

Ruby: Color = %i[red green].freeze
来源：http://vpv.hfpthk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uzc.zdbjq.cn

[G16] 对象转数组 / 字典
来源：http://uvn.zhoulong.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cul.jqgfzy.top

PHP:  get_object_vars($obj);
来源：http://hgq.jyoumei.cn

JS:   Object.entries(obj)
来源：http://fud.fktsv.cn

TS:   Object.entries(obj)
来源：http://ehj.nanxuanxn.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pen.yuanzhike.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://psb.daxiang520.top

Ruby: obj.instance_variables
来源：http://zia.gaohongyu789.top

C#:   // 用反射或 System.Text.Json
来源：http://rxb.vehdjk.com

================================================================================
来源：http://rvo.tanke756.top

H. 异常与错误处理
来源：http://pla.zycfv.cn

================================================================================
来源：http://tor.aibaodan.cn

[H01] try / catch 基础
来源：http://kth.hammf.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dlz.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tic.yonumen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wmc.ybcxt.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://scu.mhx1999.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dje.shanyushiyangtech.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ngy.cucudq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dsv.bbcook.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ylp.guowangkeji.top

[H02] finally / ensure 收尾
来源：http://unc.chenlongwang.top

Py:   try: f()⏎finally: cleanup()
来源：http://kgb.uphjek.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://dai.jiagoushi.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bkw.xinyue.icu

TS:   try { f(); } finally { cleanup(); }
来源：http://gqa.gogol.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://duu.cdnleiting.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rkv.zhaomingkeji.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://vxy.daxiang520.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rtj.sysykeji.top

[H03] 主动抛出异常
来源：http://uyk.ybcxt.top

Py:   raise ValueError("错误信息")
来源：http://wne.sufxvd.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bvt.tian-w.cn

JS:   throw new Error("错误信息");
来源：http://xmj.yonumen.top

TS:   throw new Error("错误信息");
来源：http://pde.pengpengdd.cyou

Java: throw new IllegalArgumentException("错误信息");
来源：http://olu.feifeiyinyue.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ydw.tarul.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qmc.nwbrower.top

C#:   throw new ArgumentException("错误信息");
来源：http://jwy.316326.xyz

[H04] 自定义异常类型
来源：http://oge.fktsv.cn

Py:   class MyError(Exception): pass
来源：http://oqt.cdnleiting.top

PHP:  class MyError extends RuntimeException {}
来源：http://dzk.jinqigufen.top

JS:   class MyError extends Error {}
来源：http://ncm.epnwcf.com

TS:   class MyError extends Error {}
来源：http://rzs.ybcxt.top

Java: class MyException extends RuntimeException {}
来源：http://oio.yuanzhike.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gxr.yj202588.top

Ruby: class MyError < StandardError; end
来源：http://gsk.gotoacloud.top

C#:   class MyException : Exception {}
来源：http://fxi.jinyuanbaomall.cn

[H05] 捕获特定类型
来源：http://ojs.gzhubu.top

Py:   except ValueError as e:
来源：http://qbo.cqqwz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vmc.yongpay.top

JS:   if (e instanceof TypeError) {}
来源：http://qya.yanxiufei.cn

TS:   if (e instanceof TypeError) {}
来源：http://skz.birdmap.top

Java: catch (IOException | SQLException e) {}
来源：http://zsr.wangdashe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sxu.bbcook.cn

Ruby: rescue ArgumentError => e
来源：http://enq.bjfxy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rgr.hfpthk.cn

[H06] 可选值 / 空值安全访问
来源：http://foa.feifeiyinyue.top

Py:   value = d.get("k") or default
来源：http://duh.wangdashe.top

PHP:  $v = $d["k"] ?? null;
来源：http://bmh.yvedp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://skg.svipenyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://haj.yuanzhike.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://abt.mhx1999.top

Go:   if v, ok := m["k"]; ok { }
来源：http://tkp.haohaochexian.top

Ruby: d&.dig(:a, :b)
来源：http://vdz.ppjwa.cn

C#:   obj?.A?.B ?? default
来源：http://cyb.xuanzx.com

[H07] 断言
来源：http://yvf.shuidangran.top

Py:   assert x > 0, "必须为正"
来源：http://cxa.tarul.cn

PHP:  assert($x > 0);
来源：http://ami.wangdashe.top

JS:   console.assert(x > 0);
来源：http://wsb.jlsjyb.cn

TS:   console.assert(x > 0);
来源：http://tca.ivvv.top

Java: assert x > 0 : "必须为正";
来源：http://kxn.zhongyouzk.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ybf.guowangkeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://fns.epnwcf.com

C#:   Debug.Assert(x > 0);
来源：http://snb.yangfankeji.com

[H08] 获取错误信息与堆栈
来源：http://anw.jyoumei.cn

Py:   str(e);  traceback.format_exc()
来源：http://ywd.xingfuxueyuan.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dho.cqqwz.cn

JS:   e.message;  e.stack
来源：http://ayk.zhongyouzk.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qmk.tanke756.top

Java: e.getMessage();  e.printStackTrace()
来源：http://osk.cucudq.cn

Go:   err.Error()
来源：http://ojn.jinghuilouyu.cn

Ruby: e.message;  e.backtrace
来源：http://hmy.ydzc1.top

C#:   e.Message;  e.StackTrace
来源：http://vyu.ybcxt.top

[H09] 带错误码的异常
来源：http://ahp.zhixingplan.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hqh.vqdsnc.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fog.guannengcc.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ypw.316326.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://usy.jqgufenzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rfa.wangshuangyany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kkw.yanxiufei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://baz.yj202588.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kex.gzhubu.top

[H10] 资源自动释放
来源：http://emy.dashuyun.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://god.52xcode.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eis.hywenlv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://foq.jianghu66.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lrg.jinghuilouyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wfs.shuidangran.top

Go:   defer f.Close()
来源：http://gjr.c1oappe.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yxy.52xcode.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kvn.zycfv.cn

================================================================================
来源：http://kgl.bjfxy.top

I. 正则表达式
来源：http://rjq.cdnleiting.top

================================================================================
来源：http://gfz.zdqjudy.top

[I01] 判断是否匹配
来源：http://wlj.sysykeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xtl.xziqi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tbe.ctjpmb.com

JS:   /\d+/.test(s)
来源：http://ljc.gogol.net.cn

TS:   /\d+/.test(s)
来源：http://lao.sxryk.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wei.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://llr.bbcook.cn

Ruby: s.match?(/\d+/)
来源：http://wcd.snrcjt.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mam.jinqigufen.top

[I02] 提取所有匹配
来源：http://lwa.fanxiaobao.xyz

Py:   re.findall(r"\d+", s)
来源：http://fac.yvedp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kss.aizwys.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lic.gotoacloud.top

TS:   s.match(/\d+/g)
来源：http://xrz.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ark.bbcook.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lfz.hongshengwenyu.top

Ruby: s.scan(/\d+/)
来源：http://pch.birdmap.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yqb.gogol.net.cn

[I03] 提取捕获分组
来源：http://lzw.gzhubu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://loy.cdnleiting.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nsi.ivvv.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hyz.zdqjudy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cck.chenzaomai.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ymc.nanxinkj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nat.ybcxt.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wri.9152youxi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kjg.0kj1m.cn

[I04] 正则替换
来源：http://xat.zdbjq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vsi.iojbl.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://usv.zhaomingkeji.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://dyq.xziqi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gvt.hammf.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wgf.cqqwz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qgc.jqgfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://uor.yj202588.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ayw.yangfankeji.com

[I05] 按正则拆分
来源：http://mze.yvedp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wjj.jianghu66.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cno.nanxuanxn.top

JS:   s.split(/\s*,\s*/)
来源：http://znr.hnqzz.top

TS:   s.split(/\s*,\s*/)
来源：http://fgl.daxiang520.top

Java: s.split("\\s*,\\s*")
来源：http://oao.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qqp.c1oappe.top

Ruby: s.split(/\s*,\s*/)
来源：http://tap.gzhubu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zoc.jqgfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ore.fzhhl.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lyp.smart0.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uvr.yangfankeji.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jvi.tianlin.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fxo.sxryk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zdi.xziqi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oag.aibaodan.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bah.hesvh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cqq.jqgufenzy.top

[I07] 忽略大小写与多行模式
来源：http://mlr.0kj1m.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rmd.zhongyouzk.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gfc.tianlin.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bzi.pycfn.com

TS:   /error/gim
来源：http://atc.zhijiandao.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vhe.andypj.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wfs.9152youxi.cn

Ruby: s.scan(/error/i)
来源：http://oka.zycfv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yfa.xziqi.cn

[I08] 贪婪与非贪婪匹配
来源：http://etl.jinyuanbaomall.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ydt.zhongyouzk.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jhr.jyoumei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wvl.tarul.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cxd.aibaodan.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rbc.hesvh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bew.hnqzz.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kgd.hcnkem.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ave.bbcook.cn

================================================================================
来源：http://ray.zhiwuduotai.top

J. 日期与时间
来源：http://kwx.sufxvd.cn

================================================================================
来源：http://gwg.tian-w.cn

[J01] 获取当前时间
来源：http://lfd.cqqwz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lrm.vehdjk.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ozf.gotoacloud.top

JS:   new Date();  Date.now()
来源：http://ckg.shangyingyoupin.top

TS:   new Date();  Date.now()
来源：http://hga.jqgufenzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://sus.zdbjq.cn

Go:   time.Now()
来源：http://mqa.jinghuilouyu.cn

Ruby: Time.now
来源：http://pzl.ydjk.org.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jfp.quarkkingdee.top

[J02] 格式化输出
来源：http://goe.zdqjudy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ubx.zdbjq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ioi.jqgfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xvy.ybcxt.top

TS:   d.toISOString()
来源：http://uek.nanxinkj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://omw.guannengcc.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qgq.0kj1m.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wtu.jiagoushi.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://frl.fzhhl.top

[J03] 字符串解析为日期
来源：http://zgd.zhixingplan.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vqi.9152youxi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mov.smart0.xyz

JS:   new Date("2024-01-02")
来源：http://xuq.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://iic.gzhubu.top

Java: LocalDate.parse("2024-01-02")
来源：http://czs.tian-w.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fdo.yangfankeji.com

Ruby: Date.parse("2024-01-02")
来源：http://kpc.hysaishi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ctn.xuetiantiany.cn

[J04] 时间戳与日期互转
来源：http://wpl.xylfe.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cbl.jinyuanbaomall.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tvg.jinghuilouyu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tzm.sxryk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xax.snrcjt.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zww.cashguo.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lze.pengpengdd.cyou

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hhj.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jpi.hongshengwenyu.top

[J05] 时间加减（加 7 天）
来源：http://foh.pycfn.com

Py:   now + timedelta(days=7)
来源：http://qfy.9152youxi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gcp.zhaomingkeji.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xrm.zhengqikj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rnl.zdqjudy.top

Java: LocalDate.now().plusDays(7)
来源：http://sfu.redwolf501.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fyj.jianghu66.top

Ruby: Time.now + 7 * 86400
来源：http://bud.shuidangran.top

C#:   DateTime.Now.AddDays(7)
来源：http://lbs.ivvv.top

[J06] 计算两时间之差
来源：http://kzi.sufxvd.cn

Py:   (end - start).total_seconds()
来源：http://pzw.jinghuilouyu.cn

PHP:  $end->diff($start)->days;
来源：http://vvx.52xcode.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zjn.ydjk.org.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jqk.tian-w.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fkx.hongshengwenyu.top

Go:   end.Sub(start).Hours()
来源：http://mat.ydjk.org.cn

Ruby: end - start                 # 返回秒数
来源：http://yiu.hammf.cn

C#:   (end - start).TotalSeconds
来源：http://mqv.cashguo.top

[J07] 比较两个日期
来源：http://gui.ydzc1.top

Py:   d1 < d2;  d1 == d2
来源：http://juz.tianlin.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://juz.xingfuxueyuan.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://fmu.havefunace.top

TS:   d1.getTime() < d2.getTime()
来源：http://dhk.hysaishi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://npw.hfpthk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lih.hfpthk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://piz.jiagoushi.top

C#:   d1 < d2;  d1 == d2
来源：http://ewy.meibo888.top

[J08] 提取年月日与星期
来源：http://nzu.jqgufenzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jzp.shangyingyoupin.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eib.uphjek.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ciq.chenjidiqi.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pjs.jinyuanbaomall.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hau.tanke756.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lhl.0kj1m.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oft.vqdsnc.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tds.dashuyun.cn

[J09] 时区处理
来源：http://bxg.ppjwa.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uuv.epnwcf.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://prj.jqgufenzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mfc.hysaishi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jey.fanxiaobao.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kgh.hammf.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wgo.haohaochexian.top

Ruby: Time.now.getlocal("+08:00")
来源：http://gaj.jinghuilouyu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://khv.zhaomingkeji.xyz

[J10] 取今天 / 本月第一天
来源：http://bdj.sufxvd.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cng.sysykeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nci.hesvh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jad.sjlbkw.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jhq.zhaomingkeji.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bob.cheryme.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://amu.jyoumei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oyz.epnwcf.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oeb.zycfv.cn

================================================================================
来源：http://aca.zdbjq.cn

K. JSON 与序列化
来源：http://jcn.zhijiandao.cn

================================================================================
来源：http://fyf.sufxvd.cn

[K01] 对象转 JSON 字符串
来源：http://lju.yuxming.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://htp.chenlongwang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ykq.hnqzz.top

JS:   JSON.stringify(obj)
来源：http://eok.shanyushiyangkeji.top

TS:   JSON.stringify(obj)
来源：http://wtz.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wki.meibo888.top

Go:   json.Marshal(obj)
来源：http://xdg.ivvv.top

Ruby: obj.to_json                                     // require "json"
来源：http://uaf.tanke756.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jqc.xuanzx.com

[K02] JSON 字符串转对象
来源：http://adf.svipenyu.cn

Py:   json.loads(s)
来源：http://jtt.cheryme.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://but.guowangkeji.top

JS:   JSON.parse(s)
来源：http://xrs.daxiang520.top

TS:   JSON.parse(s)
来源：http://oty.zhiwuduotai.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yrk.zhoulong.xyz

Go:   json.Unmarshal(data, &v)
来源：http://hvw.yvedp.cn

Ruby: JSON.parse(s)
来源：http://paw.sufxvd.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qff.yuxming.cn

[K03] JSON 美化输出（带缩进）
来源：http://wwu.zhaomingkeji.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oku.hammf.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://utr.hywenlv.cn


<!-- 参考信息 -->