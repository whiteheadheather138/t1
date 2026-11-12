代发 wailian999

C#:   record User(string Name, int Age);
来源：http://jdw.0kj1m.cn

[G15] 枚举
来源：http://aoj.ctjpmb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bfd.kuanghao11.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vgp.aibaodan.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kxn.nanxuanxn.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lxr.mhx1999.top

Java: enum Color { RED, GREEN }
来源：http://len.yuanzhike.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://doy.ivvv.top

Ruby: Color = %i[red green].freeze
来源：http://koh.aizwys.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ork.uphjek.com

[G16] 对象转数组 / 字典
来源：http://knb.jinyuanbaomall.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mln.xuanzx.com

PHP:  get_object_vars($obj);
来源：http://ipc.xylfe.cn

JS:   Object.entries(obj)
来源：http://imu.jinqigfzy.top

TS:   Object.entries(obj)
来源：http://fnn.jinqigfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lss.meibo888.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://cim.shanyushiyangtech.top

Ruby: obj.instance_variables
来源：http://yuy.zhoulong.xyz

C#:   // 用反射或 System.Text.Json
来源：http://sdf.quarkkingdee.top

================================================================================
来源：http://wdm.zhixingplan.top

H. 异常与错误处理
来源：http://aaw.yuanzhike.top

================================================================================
来源：http://mmc.xuanzx.com

[H01] try / catch 基础
来源：http://kqq.nanxuanxn.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ugx.ydjk.org.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://phs.hesvh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://akp.sysykeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tee.dianchejie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hgh.sysykeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rbo.pycfn.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uxe.yangfankeji.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ggy.jinghuilouyu.cn

[H02] finally / ensure 收尾
来源：http://lcg.xinyue.icu

Py:   try: f()⏎finally: cleanup()
来源：http://wxp.vqdsnc.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gyq.wangshuangyany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://drd.jiagoushi.top

TS:   try { f(); } finally { cleanup(); }
来源：http://cjl.hcnkem.com

Java: try { f(); } finally { cleanup(); }
来源：http://ztg.fzhhl.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wuk.aibaodan.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bvc.jinghuilouyu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sza.jiagoushi.top

[H03] 主动抛出异常
来源：http://nfb.yonumen.top

Py:   raise ValueError("错误信息")
来源：http://box.zhoulong.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nfh.yj202588.top

JS:   throw new Error("错误信息");
来源：http://kdj.jlsjyb.cn

TS:   throw new Error("错误信息");
来源：http://iro.hfpthk.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cei.jinyuanbaomall.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://odt.jianghu66.top

Ruby: raise ArgumentError, "错误信息"
来源：http://feu.tianlin.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://esv.hysaishi.cn

[H04] 自定义异常类型
来源：http://vgg.daxiang520.top

Py:   class MyError(Exception): pass
来源：http://diz.yonumen.top

PHP:  class MyError extends RuntimeException {}
来源：http://ywx.cqqwz.cn

JS:   class MyError extends Error {}
来源：http://evi.nanxuanxn.top

TS:   class MyError extends Error {}
来源：http://krf.tanke756.top

Java: class MyException extends RuntimeException {}
来源：http://uru.yangfankeji.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dze.dianchejie.cn

Ruby: class MyError < StandardError; end
来源：http://yuo.yj20258888.top

C#:   class MyException : Exception {}
来源：http://iht.tian-w.cn

[H05] 捕获特定类型
来源：http://emw.c1oappe.top

Py:   except ValueError as e:
来源：http://djh.jyoumei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dji.0kj1m.cn

JS:   if (e instanceof TypeError) {}
来源：http://yxj.yanxiufei.cn

TS:   if (e instanceof TypeError) {}
来源：http://ooh.ctjpmb.com

Java: catch (IOException | SQLException e) {}
来源：http://kbf.wangshuangyany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://akt.jqgfzy.top

Ruby: rescue ArgumentError => e
来源：http://onk.zhaomingkeji.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lap.fengsongda.top

[H06] 可选值 / 空值安全访问
来源：http://faz.hongshengwenyu.top

Py:   value = d.get("k") or default
来源：http://bwa.ppjwa.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mja.gogol.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://iqc.gotoacloud.top

TS:   obj?.a?.b;  d ?? default
来源：http://wtp.wangdashe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sow.xinyue.icu

Go:   if v, ok := m["k"]; ok { }
来源：http://yat.ivvv.top

Ruby: d&.dig(:a, :b)
来源：http://gec.havefunace.top

C#:   obj?.A?.B ?? default
来源：http://zgx.ybcxt.top

[H07] 断言
来源：http://wzv.zhijiandao.cn

Py:   assert x > 0, "必须为正"
来源：http://mev.aizwys.cn

PHP:  assert($x > 0);
来源：http://tio.yangfankeji.com

JS:   console.assert(x > 0);
来源：http://edx.fktsv.cn

TS:   console.assert(x > 0);
来源：http://gwa.316326.xyz

Java: assert x > 0 : "必须为正";
来源：http://hnc.jyoumei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lys.ydjk.org.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kkc.nanxuanxn.top

C#:   Debug.Assert(x > 0);
来源：http://gua.xuanzx.com

[H08] 获取错误信息与堆栈
来源：http://hyz.hywenlv.cn

Py:   str(e);  traceback.format_exc()
来源：http://ffp.52xcode.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gez.nanxuanxn.top

JS:   e.message;  e.stack
来源：http://ifq.jqgfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://nlh.haohaochexian.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xsu.havefunace.top

Go:   err.Error()
来源：http://qsg.chenjidiqi.icu

Ruby: e.message;  e.backtrace
来源：http://lek.guowangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://udw.zhoulong.xyz

[H09] 带错误码的异常
来源：http://kcn.yfazqb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bqg.zycfv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yze.xylfe.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hrm.nwbrower.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xvc.yuanzhike.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://duv.hcnkem.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wwz.zhiwuduotai.top

Ruby: raise MyError.new("fail", 500)
来源：http://soa.cashguo.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fcl.ydzc1.top

[H10] 资源自动释放
来源：http://hbx.pengpengdd.cyou

Py:   with open("a.txt") as f: data = f.read()
来源：http://uya.jlsjyb.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://trv.jinqigfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eyq.hongshengwenyu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mqm.fzhhl.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pan.shanyushiyangkeji.top

Go:   defer f.Close()
来源：http://tnk.zdbjq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lyo.svipenyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://etm.cdnleiting.top

================================================================================
来源：http://svv.zhongyouzk.top

I. 正则表达式
来源：http://hbo.sufxvd.cn

================================================================================
来源：http://ejc.daxiang520.top

[I01] 判断是否匹配
来源：http://qsi.redwolf501.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wyv.chenjidiqi.icu

PHP:  preg_match('/\d+/', $s);
来源：http://mvk.shanyushiyangtech.top

JS:   /\d+/.test(s)
来源：http://hln.nanxuanxn.top

TS:   /\d+/.test(s)
来源：http://bwa.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iah.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wbp.ppjwa.cn

Ruby: s.match?(/\d+/)
来源：http://uor.yuxming.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ttu.chenlongwang.top

[I02] 提取所有匹配
来源：http://mhx.fzhhl.top

Py:   re.findall(r"\d+", s)
来源：http://clu.shzxlz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fau.pycfn.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ooa.mhx1999.top

TS:   s.match(/\d+/g)
来源：http://gvo.9152youxi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nto.andypj.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cza.zhongyouzk.top

Ruby: s.scan(/\d+/)
来源：http://yas.meibo888.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rkh.yj20258.top

[I03] 提取捕获分组
来源：http://kac.cucudq.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hbs.hesvh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hqs.daria6918.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tfy.yangfankeji.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wnk.jyoumei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ecv.gaohongyu789.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wcn.hywenlv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://phe.zhijiandao.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cza.svipenyu.cn

[I04] 正则替换
来源：http://oic.ydzc1.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vid.pengpengdd.cyou

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bcq.wangdashe.top

JS:   s.replace(/\d+/g, "#")
来源：http://oxq.tian-w.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gtd.zdqjudy.top

Java: s.replaceAll("\\d+", "#")
来源：http://gmz.0kj1m.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ecf.fengsongda.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nwd.birdmap.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fcj.yonumen.top

[I05] 按正则拆分
来源：http://sml.tianlin.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://zlf.ybcxt.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sdv.yj20258.top

JS:   s.split(/\s*,\s*/)
来源：http://klm.bjfxy.top

TS:   s.split(/\s*,\s*/)
来源：http://lwz.sweek.top

Java: s.split("\\s*,\\s*")
来源：http://pii.gzhubu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://urk.9152youxi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ivd.yj202588.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zbu.zhaomingkeji.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zag.nanxuanxn.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cxu.shuidangran.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qxp.jinyuanbaomall.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kjg.cdnleiting.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bty.jianghu66.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mni.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wpq.52xcode.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xwx.yuxming.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://prh.yuxming.cn

[I07] 忽略大小写与多行模式
来源：http://fbx.zdbjq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ynp.gotoacloud.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nne.fengsongda.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cbj.jinqigufen.top

TS:   /error/gim
来源：http://zxl.havefunace.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ykw.chenlongwang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://auv.aibaodan.cn

Ruby: s.scan(/error/i)
来源：http://evc.tanke756.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bft.xuetiantiany.cn

[I08] 贪婪与非贪婪匹配
来源：http://ntx.cdnleiting.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://knc.zdqjudy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zoc.yuxming.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ylg.fktsv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://edh.ehwqpu.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://spc.sufxvd.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gkw.jinghuilouyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yye.gaohongyu789.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://veg.xylfe.cn

================================================================================
来源：http://fwv.ivvv.top

J. 日期与时间
来源：http://glg.nanxinkj.top

================================================================================
来源：http://ccn.meibo888.top

[J01] 获取当前时间
来源：http://fze.vqdsnc.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bcc.cucudq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oqb.sjlbkw.cn

JS:   new Date();  Date.now()
来源：http://gdp.feifeiyinyue.top

TS:   new Date();  Date.now()
来源：http://sjn.xziqi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nxr.wangdashe.top

Go:   time.Now()
来源：http://bka.nanxinkj.top

Ruby: Time.now
来源：http://riz.fengsongda.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://stx.jianghu66.top

[J02] 格式化输出
来源：http://hli.yanxiufei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xeq.9152youxi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tgc.ppjwa.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bbx.epnwcf.com

TS:   d.toISOString()
来源：http://uka.andypj.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cpc.gotoacloud.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hyr.hammf.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xhh.dashuyun.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jth.mhx1999.top

[J03] 字符串解析为日期
来源：http://etc.feifeiyinyue.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wms.kuanghao11.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bfs.wangdashe.top

JS:   new Date("2024-01-02")
来源：http://zvj.yvedp.cn

TS:   new Date("2024-01-02")
来源：http://fbr.andypj.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://amn.yj20258.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bxr.zdbjq.cn

Ruby: Date.parse("2024-01-02")
来源：http://hhf.pycfn.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wzb.meibo888.top

[J04] 时间戳与日期互转
来源：http://wbh.epnwcf.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xuw.sysykeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mdf.ppjwa.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cds.gaohongyu789.top

TS:   Math.floor(Date.now() / 1000)
来源：http://czi.ydjk.org.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lmq.jinyuanbaomall.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vvu.aibaodan.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oyv.sweek.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eew.ybcxt.top

[J05] 时间加减（加 7 天）
来源：http://bhz.fktsv.cn

Py:   now + timedelta(days=7)
来源：http://jth.jinghuilouyu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nit.jinqigfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://onw.chenlongwang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uov.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://erj.shangyingyoupin.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://exs.sysykeji.top

Ruby: Time.now + 7 * 86400
来源：http://ifx.svipenyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ykh.jlsjyb.cn

[J06] 计算两时间之差
来源：http://iql.fzhhl.top

Py:   (end - start).total_seconds()
来源：http://aqd.svipenyu.cn

PHP:  $end->diff($start)->days;
来源：http://txx.sysykeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ubu.xylfe.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qit.vqdsnc.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jgz.xuetiantiany.cn

Go:   end.Sub(start).Hours()
来源：http://fyq.aizwys.cn

Ruby: end - start                 # 返回秒数
来源：http://het.ehwqpu.com

C#:   (end - start).TotalSeconds
来源：http://ypf.yanxiufei.cn

[J07] 比较两个日期
来源：http://mdt.jlsjyb.cn

Py:   d1 < d2;  d1 == d2
来源：http://qio.yj20258.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tfh.guannengcc.top

JS:   d1.getTime() < d2.getTime()
来源：http://jpt.sufxvd.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bhe.haohaochexian.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ppy.xylfe.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vlr.guannengcc.top

Ruby: d1 < d2;  d1 == d2
来源：http://cwv.shzxlz.cn

C#:   d1 < d2;  d1 == d2
来源：http://bkg.cucudq.cn

[J08] 提取年月日与星期
来源：http://ept.cucudq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lkn.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://apa.sjlbkw.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://adu.guowangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gxt.nanxinkj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nvx.52xcode.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kvz.zhengqikj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://osj.ppjwa.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bhg.fehbvm.com

[J09] 时区处理
来源：http://wpi.hysaishi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://imw.fzhhl.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bhk.ivvv.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nwg.fanxiaobao.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dxq.smart0.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jnw.jinqigufen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sck.fzhhl.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lyi.gzhubu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zwv.snrcjt.cn

[J10] 取今天 / 本月第一天
来源：http://gyu.wangshuangyany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jjw.xziqi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zlp.316326.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mtn.jyoumei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://erp.ybcxt.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dox.cashguo.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tdu.yj20258888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lfq.dianchejie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dgp.yj20258888.top

================================================================================
来源：http://vwe.xinyue.icu

K. JSON 与序列化
来源：http://obp.meibo888.top

================================================================================
来源：http://ico.nanxuanxn.top

[K01] 对象转 JSON 字符串
来源：http://cne.yfazqb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fbp.hnqzz.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wvf.snrcjt.cn

JS:   JSON.stringify(obj)
来源：http://vyj.c1oappe.top

TS:   JSON.stringify(obj)
来源：http://wqn.chenzaomai.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dbg.hywenlv.cn

Go:   json.Marshal(obj)
来源：http://tcy.guannengcc.top

Ruby: obj.to_json                                     // require "json"
来源：http://wrv.c1oappe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://pkr.ywan-chungtsiang.top

[K02] JSON 字符串转对象
来源：http://snv.shuidangran.top

Py:   json.loads(s)
来源：http://pqy.epnwcf.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bsx.xuetiantiany.cn

JS:   JSON.parse(s)
来源：http://jwy.tian-w.cn

TS:   JSON.parse(s)
来源：http://ayu.birdmap.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ayo.yj20258888.top

Go:   json.Unmarshal(data, &v)
来源：http://hxz.yfazqb.com

Ruby: JSON.parse(s)
来源：http://lpb.shzxlz.cn


<!-- 参考信息 -->