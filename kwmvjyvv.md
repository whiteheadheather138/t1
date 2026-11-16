代发 wailian999

C#:   record User(string Name, int Age);
来源：http://fjl.zhijiandao.cn

[G15] 枚举
来源：http://sku.c1oappe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pdo.0kj1m.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jjl.gogol.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://owm.andypj.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://aov.yj202588.top

Java: enum Color { RED, GREEN }
来源：http://aka.chenlongwang.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://twq.quarkkingdee.top

Ruby: Color = %i[red green].freeze
来源：http://gjt.yvedp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tkh.ctjpmb.com

[G16] 对象转数组 / 字典
来源：http://jnz.jlsjyb.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xeu.hywenlv.cn

PHP:  get_object_vars($obj);
来源：http://onu.fehbvm.com

JS:   Object.entries(obj)
来源：http://mwn.shangyingyoupin.top

TS:   Object.entries(obj)
来源：http://sta.cashguo.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://iar.zhijiandao.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rnf.shanyushiyangkeji.top

Ruby: obj.instance_variables
来源：http://ckj.yongpay.top

C#:   // 用反射或 System.Text.Json
来源：http://iob.jinghuilouyu.cn

================================================================================
来源：http://ips.yonumen.top

H. 异常与错误处理
来源：http://jpf.guannengcc.top

================================================================================
来源：http://esd.birdmap.top

[H01] try / catch 基础
来源：http://gxq.vqdsnc.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lvh.ctjpmb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://otr.jinyuanbaomall.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wgc.hnxiangtu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oet.jinyuanbaomall.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sku.fanxiaobao.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qqj.cqqwz.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gfh.hcnkem.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qmc.vehdjk.com

[H02] finally / ensure 收尾
来源：http://vol.gogol.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jqq.shuidangran.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://idd.vehdjk.com

JS:   try { f(); } finally { cleanup(); }
来源：http://pnb.zhengqikj.top

TS:   try { f(); } finally { cleanup(); }
来源：http://fiy.haohaochexian.top

Java: try { f(); } finally { cleanup(); }
来源：http://lje.xuetiantiany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ydq.wangshuangyany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://udg.fengsongda.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://aif.yueranfly.top

[H03] 主动抛出异常
来源：http://ixw.iojbl.cn

Py:   raise ValueError("错误信息")
来源：http://pim.nanxuanxn.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nbs.smart0.xyz

JS:   throw new Error("错误信息");
来源：http://twr.jianghu66.top

TS:   throw new Error("错误信息");
来源：http://dmy.xuetiantiany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dtl.xuanzx.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ghy.bbcook.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lqy.0kj1m.cn

C#:   throw new ArgumentException("错误信息");
来源：http://edt.birdmap.top

[H04] 自定义异常类型
来源：http://ycv.fanxiaobao.xyz

Py:   class MyError(Exception): pass
来源：http://hci.cashguo.top

PHP:  class MyError extends RuntimeException {}
来源：http://ips.shanyushiyangkeji.top

JS:   class MyError extends Error {}
来源：http://utw.zhoulong.xyz

TS:   class MyError extends Error {}
来源：http://pib.jinqigufen.top

Java: class MyException extends RuntimeException {}
来源：http://gff.yvedp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ajb.9152youxi.cn

Ruby: class MyError < StandardError; end
来源：http://zqh.tanke756.top

C#:   class MyException : Exception {}
来源：http://hnx.cucudq.cn

[H05] 捕获特定类型
来源：http://sgb.yonumen.top

Py:   except ValueError as e:
来源：http://mkl.hnxiangtu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mrm.daxiang520.top

JS:   if (e instanceof TypeError) {}
来源：http://rzj.shanyushiyangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://nch.zycfv.cn

Java: catch (IOException | SQLException e) {}
来源：http://kzt.guannengcc.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://knb.sysykeji.top

Ruby: rescue ArgumentError => e
来源：http://jhp.jinqigufen.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lrk.sufxvd.cn

[H06] 可选值 / 空值安全访问
来源：http://jbi.jqgfzy.top

Py:   value = d.get("k") or default
来源：http://vyh.yvedp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gkb.gzhubu.top

JS:   obj?.a?.b;  d ?? default
来源：http://ctz.redwolf501.top

TS:   obj?.a?.b;  d ?? default
来源：http://ivg.hcnkem.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rxq.jinqigufen.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kou.epnwcf.com

Ruby: d&.dig(:a, :b)
来源：http://wzd.0kj1m.cn

C#:   obj?.A?.B ?? default
来源：http://wvq.jinqigufen.top

[H07] 断言
来源：http://zat.bjfxy.top

Py:   assert x > 0, "必须为正"
来源：http://xen.guannengcc.top

PHP:  assert($x > 0);
来源：http://xpn.fehbvm.com

JS:   console.assert(x > 0);
来源：http://qvc.ctjpmb.com

TS:   console.assert(x > 0);
来源：http://bkp.gzhubu.top

Java: assert x > 0 : "必须为正";
来源：http://prq.shangyingyoupin.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xoo.zhiwuduotai.top

Ruby: raise "必须为正" unless x > 0
来源：http://uhw.ydzc1.top

C#:   Debug.Assert(x > 0);
来源：http://sik.shanyushiyangtech.top

[H08] 获取错误信息与堆栈
来源：http://ymi.quarkkingdee.top

Py:   str(e);  traceback.format_exc()
来源：http://nzm.chenjidiqi.icu

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tjo.jianghu66.top

JS:   e.message;  e.stack
来源：http://gwz.meibo888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://uvz.hammf.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uiv.c1oappe.top

Go:   err.Error()
来源：http://zmg.havefunace.top

Ruby: e.message;  e.backtrace
来源：http://tqz.daxiang520.top

C#:   e.Message;  e.StackTrace
来源：http://kgb.svipenyu.cn

[H09] 带错误码的异常
来源：http://owa.aibaodan.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iyw.jinqigfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qya.ppjwa.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tfq.hnqzz.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wub.daxiang520.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hai.shanyushiyangtech.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://esm.dashuyun.cn

Ruby: raise MyError.new("fail", 500)
来源：http://eic.yfazqb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://zie.ehwqpu.com

[H10] 资源自动释放
来源：http://fpq.zdbjq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mjz.gogol.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fpp.0kj1m.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://njj.hongshengwenyu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bix.hammf.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qvz.xinyue.icu

Go:   defer f.Close()
来源：http://ekm.sxryk.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oye.ehwqpu.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qvk.pycfn.com

================================================================================
来源：http://mub.shanyushiyangtech.top

I. 正则表达式
来源：http://bjy.redwolf501.top

================================================================================
来源：http://cux.vehdjk.com

[I01] 判断是否匹配
来源：http://cuh.xziqi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kqp.cqqwz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pop.cucudq.cn

JS:   /\d+/.test(s)
来源：http://apy.havefunace.top

TS:   /\d+/.test(s)
来源：http://uqe.yuxming.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pxh.xinyue.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cai.zhixingplan.top

Ruby: s.match?(/\d+/)
来源：http://yzg.hcnkem.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pzz.ehwqpu.com

[I02] 提取所有匹配
来源：http://amf.mhx1999.top

Py:   re.findall(r"\d+", s)
来源：http://cuv.zycfv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://waw.yfazqb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pok.fzhhl.top

TS:   s.match(/\d+/g)
来源：http://rus.hysaishi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hgz.daxiang520.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ewc.xuetiantiany.cn

Ruby: s.scan(/\d+/)
来源：http://evh.pycfn.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hxm.wangdashe.top

[I03] 提取捕获分组
来源：http://xfw.jqgufenzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dsy.shzxlz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pwj.hnqzz.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fam.sweek.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uvc.wangdashe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xww.cqqwz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ayy.jiagoushi.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ghh.zhiwuduotai.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zgw.epnwcf.com

[I04] 正则替换
来源：http://qrr.jyoumei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wuk.yonumen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yoh.yongpay.top

JS:   s.replace(/\d+/g, "#")
来源：http://hdg.zhongyouzk.top

TS:   s.replace(/\d+/g, "#")
来源：http://xhp.c1oappe.top

Java: s.replaceAll("\\d+", "#")
来源：http://kmc.316326.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://nvf.c1oappe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://sfx.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fgk.fzhhl.top

[I05] 按正则拆分
来源：http://unl.jyoumei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dum.zycfv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kcj.yonumen.top

JS:   s.split(/\s*,\s*/)
来源：http://aly.birdmap.top

TS:   s.split(/\s*,\s*/)
来源：http://qby.dianchejie.cn

Java: s.split("\\s*,\\s*")
来源：http://sqz.zhiwuduotai.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pyj.meibo888.top

Ruby: s.split(/\s*,\s*/)
来源：http://hiq.ivvv.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yyn.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://guu.chenjidiqi.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qsv.hywenlv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qxl.yfazqb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oll.jianghu66.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mju.wangshuangyany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rbv.redwolf501.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qkt.meibo888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rkm.jinyuanbaomall.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://poa.xylfe.cn

[I07] 忽略大小写与多行模式
来源：http://yxb.yvedp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eia.ydjk.org.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jvj.nwbrower.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vwl.ywan-chungtsiang.top

TS:   /error/gim
来源：http://amx.yanxiufei.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wqg.zhengqikj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ugj.epnwcf.com

Ruby: s.scan(/error/i)
来源：http://bvc.feifeiyinyue.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jwp.xingfuxueyuan.xyz

[I08] 贪婪与非贪婪匹配
来源：http://ofu.hysaishi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vqi.fzhhl.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://omf.xinyue.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://che.chenjidiqi.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kzy.gogol.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lsi.yongpay.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rdd.pengpengdd.cyou

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bjm.yonumen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bja.shanyushiyangtech.top

================================================================================
来源：http://wcj.zhiwuduotai.top

J. 日期与时间
来源：http://aek.xingfuxueyuan.xyz

================================================================================
来源：http://ykw.jlsjyb.cn

[J01] 获取当前时间
来源：http://dhd.yuxming.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uev.sweek.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sqv.jqgfzy.top

JS:   new Date();  Date.now()
来源：http://bzn.zhiwuduotai.top

TS:   new Date();  Date.now()
来源：http://ajo.haohaochexian.top

Java: LocalDateTime.now();  Instant.now()
来源：http://tzf.sufxvd.cn

Go:   time.Now()
来源：http://off.zdbjq.cn

Ruby: Time.now
来源：http://hlo.fzhhl.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pdh.wangdashe.top

[J02] 格式化输出
来源：http://jlu.tanke756.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://exd.jqgufenzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lec.jinqigufen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oaq.cucudq.cn

TS:   d.toISOString()
来源：http://lqw.fanxiaobao.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ayx.bbcook.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fty.pycfn.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://avb.yfazqb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bjs.gaohongyu789.top

[J03] 字符串解析为日期
来源：http://rdz.shanyushiyangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ksl.jqgufenzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hmw.xingfuxueyuan.xyz

JS:   new Date("2024-01-02")
来源：http://xxo.sjlbkw.cn

TS:   new Date("2024-01-02")
来源：http://dab.jinqigufen.top

Java: LocalDate.parse("2024-01-02")
来源：http://dki.fzhhl.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xtj.tarul.cn

Ruby: Date.parse("2024-01-02")
来源：http://brz.fzhhl.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hli.yuanzhike.top

[J04] 时间戳与日期互转
来源：http://mmk.cucudq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tth.yfazqb.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ueh.xuanzx.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lhv.chenjidiqi.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://cfs.hcnkem.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lnp.vehdjk.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kjy.ydzc1.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cvu.jinghuilouyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gwn.hysaishi.cn

[J05] 时间加减（加 7 天）
来源：http://eja.zhongyouzk.top

Py:   now + timedelta(days=7)
来源：http://wiw.jinyuanbaomall.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ghv.nanxinkj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mcf.ydjk.org.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://woe.cqqwz.cn

Java: LocalDate.now().plusDays(7)
来源：http://ugi.cdnleiting.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hul.jyoumei.cn

Ruby: Time.now + 7 * 86400
来源：http://zgk.jianghu66.top

C#:   DateTime.Now.AddDays(7)
来源：http://oqw.yj202588.top

[J06] 计算两时间之差
来源：http://bcj.xziqi.cn

Py:   (end - start).total_seconds()
来源：http://dmx.zhengqikj.top

PHP:  $end->diff($start)->days;
来源：http://cpm.redwolf501.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rcj.vehdjk.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ubn.jqgufenzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://vpf.yj20258.top

Go:   end.Sub(start).Hours()
来源：http://cfc.gogol.net.cn

Ruby: end - start                 # 返回秒数
来源：http://ghv.svipenyu.cn

C#:   (end - start).TotalSeconds
来源：http://hza.hammf.cn

[J07] 比较两个日期
来源：http://vbs.yonumen.top

Py:   d1 < d2;  d1 == d2
来源：http://rlc.smart0.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ukd.mhx1999.top

JS:   d1.getTime() < d2.getTime()
来源：http://ypn.yj20258888.top

TS:   d1.getTime() < d2.getTime()
来源：http://ohm.nwbrower.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pjg.9152youxi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hnh.birdmap.top

Ruby: d1 < d2;  d1 == d2
来源：http://hps.c1oappe.top

C#:   d1 < d2;  d1 == d2
来源：http://sby.shanyushiyangkeji.top

[J08] 提取年月日与星期
来源：http://vir.ppjwa.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gkj.ppjwa.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cgf.guowangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kwk.hammf.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qcb.jqgfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xiv.zhaomingkeji.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wvt.uphjek.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cqk.kuanghao11.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ibv.hongshengwenyu.top

[J09] 时区处理
来源：http://yab.fzhhl.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jbf.jinyuanbaomall.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jqy.hfpthk.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://avi.guowangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xrx.xingfuxueyuan.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cig.ydzc1.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vqy.guannengcc.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hrx.ybcxt.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lbz.gzhubu.top

[J10] 取今天 / 本月第一天
来源：http://nnf.xylfe.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pvx.yuanzhike.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://upr.hesvh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fgg.fanxiaobao.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cgw.sysykeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hws.zycfv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fbc.gotoacloud.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://czn.jinghuilouyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iuv.yuanzhike.top

================================================================================
来源：http://lde.hysaishi.cn

K. JSON 与序列化
来源：http://cta.yuxming.cn

================================================================================
来源：http://tia.fehbvm.com

[K01] 对象转 JSON 字符串
来源：http://web.meibo888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ibj.uphjek.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hck.fehbvm.com

JS:   JSON.stringify(obj)
来源：http://emo.hongshengwenyu.top

TS:   JSON.stringify(obj)
来源：http://zdi.yangfankeji.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gke.fehbvm.com

Go:   json.Marshal(obj)
来源：http://gbi.tarul.cn

Ruby: obj.to_json                                     // require "json"
来源：http://car.iojbl.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://taa.xingfuxueyuan.xyz

[K02] JSON 字符串转对象
来源：http://eni.zdbjq.cn

Py:   json.loads(s)
来源：http://yuu.52xcode.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oqn.52xcode.cn

JS:   JSON.parse(s)
来源：http://ygq.hcnkem.com

TS:   JSON.parse(s)
来源：http://pob.shanyushiyangtech.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vhb.redwolf501.top

Go:   json.Unmarshal(data, &v)
来源：http://vph.jinghuilouyu.cn

Ruby: JSON.parse(s)
来源：http://rlh.wangshuangyany.cn


<!-- 参考信息 -->