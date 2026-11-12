代发 wailian999

[G14] 数据类 / record
来源：http://usg.vqdsnc.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dpq.fzhhl.top

PHP:  // 用 readonly 属性模拟
来源：http://zwn.fzhhl.top

JS:   // 无内置：普通类或对象字面量
来源：http://pjx.ydzc1.top

TS:   type User = { name: string; age: number };
来源：http://qzy.sweek.top

Java: record User(String name, int age) {}
来源：http://mku.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://ucv.shangyingyoupin.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://aef.zhengqikj.top

C#:   record User(string Name, int Age);
来源：http://okx.wangdashe.top

[G15] 枚举
来源：http://lfj.yuxming.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kdj.yfazqb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://ogh.yanxiufei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qps.iojbl.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fdj.fktsv.cn

Java: enum Color { RED, GREEN }
来源：http://hug.yj20258.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pku.cucudq.cn

Ruby: Color = %i[red green].freeze
来源：http://guh.xziqi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://krk.yanxiufei.cn

[G16] 对象转数组 / 字典
来源：http://uog.zhixingplan.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ium.ybcxt.top

PHP:  get_object_vars($obj);
来源：http://jgd.nwbrower.top

JS:   Object.entries(obj)
来源：http://kkb.tanke756.top

TS:   Object.entries(obj)
来源：http://kmf.xylfe.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rph.shanyushiyangtech.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://soi.tianlin.xyz

Ruby: obj.instance_variables
来源：http://qyo.shzxlz.cn

C#:   // 用反射或 System.Text.Json
来源：http://vxu.ydjk.org.cn

================================================================================
来源：http://ocy.jiagoushi.top

H. 异常与错误处理
来源：http://aow.tanke756.top

================================================================================
来源：http://nzz.nwbrower.top

[H01] try / catch 基础
来源：http://rfp.wangshuangyany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qgt.zhixingplan.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ldb.uphjek.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tqk.zycfv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://txj.tanke756.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tvh.gaohongyu789.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iax.zhaomingkeji.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://neg.jqgufenzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kul.yvedp.cn

[H02] finally / ensure 收尾
来源：http://xuz.xinyue.icu

Py:   try: f()⏎finally: cleanup()
来源：http://zaq.fktsv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bog.xinyue.icu

JS:   try { f(); } finally { cleanup(); }
来源：http://nqr.ctjpmb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://nzp.dianchejie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uvi.daria6918.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nxx.hongshengwenyu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fux.pycfn.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://cnr.jinqigufen.top

[H03] 主动抛出异常
来源：http://uqa.yuxming.cn

Py:   raise ValueError("错误信息")
来源：http://zom.ydzc1.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gco.yonumen.top

JS:   throw new Error("错误信息");
来源：http://emn.hammf.cn

TS:   throw new Error("错误信息");
来源：http://zay.sxryk.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://axm.tianlin.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ldj.bjfxy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://bid.jqgufenzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://xhr.chenzaomai.com

[H04] 自定义异常类型
来源：http://xci.daxiang520.top

Py:   class MyError(Exception): pass
来源：http://ija.gzhubu.top

PHP:  class MyError extends RuntimeException {}
来源：http://epf.hnxiangtu.top

JS:   class MyError extends Error {}
来源：http://zxy.kuanghao11.cn

TS:   class MyError extends Error {}
来源：http://byb.tarul.cn

Java: class MyException extends RuntimeException {}
来源：http://dpq.jinqigufen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vpx.zycfv.cn

Ruby: class MyError < StandardError; end
来源：http://qli.zhijiandao.cn

C#:   class MyException : Exception {}
来源：http://mdb.xingfuxueyuan.xyz

[H05] 捕获特定类型
来源：http://nsc.yangfankeji.com

Py:   except ValueError as e:
来源：http://zqb.zhaomingkeji.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gsr.shanyushiyangtech.top

JS:   if (e instanceof TypeError) {}
来源：http://jrr.ydjk.org.cn

TS:   if (e instanceof TypeError) {}
来源：http://rel.bbcook.cn

Java: catch (IOException | SQLException e) {}
来源：http://ajr.cqqwz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fot.aibaodan.cn

Ruby: rescue ArgumentError => e
来源：http://nrk.bjfxy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zee.guowangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://nmu.sxryk.cn

Py:   value = d.get("k") or default
来源：http://lsn.jqgufenzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://ppd.ywan-chungtsiang.top

JS:   obj?.a?.b;  d ?? default
来源：http://bzh.vqdsnc.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qys.ivvv.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tro.gogol.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ade.gzhubu.top

Ruby: d&.dig(:a, :b)
来源：http://fca.ybcxt.top

C#:   obj?.A?.B ?? default
来源：http://ovr.cashguo.top

[H07] 断言
来源：http://yst.sxryk.cn

Py:   assert x > 0, "必须为正"
来源：http://xvl.yj202588.top

PHP:  assert($x > 0);
来源：http://vbd.jinghuilouyu.cn

JS:   console.assert(x > 0);
来源：http://dvc.daxiang520.top

TS:   console.assert(x > 0);
来源：http://idj.tanke756.top

Java: assert x > 0 : "必须为正";
来源：http://lqb.snrcjt.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eri.cashguo.top

Ruby: raise "必须为正" unless x > 0
来源：http://tpa.fengsongda.top

C#:   Debug.Assert(x > 0);
来源：http://qjh.gzhubu.top

[H08] 获取错误信息与堆栈
来源：http://gcg.wangshuangyany.cn

Py:   str(e);  traceback.format_exc()
来源：http://ekk.sysykeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dng.ybcxt.top

JS:   e.message;  e.stack
来源：http://mqm.ydzc1.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://thm.daria6918.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gql.zhixingplan.top

Go:   err.Error()
来源：http://wdt.yanxiufei.cn

Ruby: e.message;  e.backtrace
来源：http://fae.cdnleiting.top

C#:   e.Message;  e.StackTrace
来源：http://hqo.iojbl.cn

[H09] 带错误码的异常
来源：http://vwz.yonumen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dsn.yonumen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ptj.sjlbkw.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mdy.xingfuxueyuan.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gyo.sjlbkw.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dyv.yuanzhike.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sss.jqgfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://mkt.hammf.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pnd.pycfn.com

[H10] 资源自动释放
来源：http://oxi.cucudq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yrz.snrcjt.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lyw.daria6918.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://whk.ehwqpu.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hsw.yj20258888.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://krf.gzhubu.top

Go:   defer f.Close()
来源：http://zqw.ydzc1.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iml.316326.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ltq.ybcxt.top

================================================================================
来源：http://dyg.fehbvm.com

I. 正则表达式
来源：http://ywf.dashuyun.cn

================================================================================
来源：http://tda.hywenlv.cn

[I01] 判断是否匹配
来源：http://nmm.zhengqikj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qvm.jiagoushi.top

PHP:  preg_match('/\d+/', $s);
来源：http://oex.ydjk.org.cn

JS:   /\d+/.test(s)
来源：http://vlr.uphjek.com

TS:   /\d+/.test(s)
来源：http://wth.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dpp.cashguo.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dsl.hesvh.cn

Ruby: s.match?(/\d+/)
来源：http://xno.xylfe.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://aru.zhoulong.xyz

[I02] 提取所有匹配
来源：http://qaf.cheryme.top

Py:   re.findall(r"\d+", s)
来源：http://kwo.xuanzx.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dnk.yj20258.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sbw.316326.xyz

TS:   s.match(/\d+/g)
来源：http://xke.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://txq.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bpn.nanxuanxn.top

Ruby: s.scan(/\d+/)
来源：http://jlh.cucudq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qqf.xziqi.cn

[I03] 提取捕获分组
来源：http://yqp.zhongyouzk.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lvy.sjlbkw.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://snr.tianlin.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nxw.yueranfly.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pyl.guowangkeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xax.cdnleiting.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://amg.shangyingyoupin.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xqa.yj202588.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ufa.xingfuxueyuan.xyz

[I04] 正则替换
来源：http://epq.hnqzz.top

Py:   re.sub(r"\d+", "#", s)
来源：http://sgm.cdnleiting.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ftd.sjlbkw.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ckh.yanxiufei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rre.meibo888.top

Java: s.replaceAll("\\d+", "#")
来源：http://cbk.shuidangran.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bjl.ydjk.org.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xsq.shanyushiyangtech.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fjq.shzxlz.cn

[I05] 按正则拆分
来源：http://jgg.sysykeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zjk.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://joo.sxryk.cn

JS:   s.split(/\s*,\s*/)
来源：http://coa.ywan-chungtsiang.top

TS:   s.split(/\s*,\s*/)
来源：http://lix.andypj.xyz

Java: s.split("\\s*,\\s*")
来源：http://fre.yonumen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://esq.zhijiandao.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rda.nanxinkj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ict.zhongyouzk.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jhj.jianghu66.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vtp.fehbvm.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fzg.zhengqikj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ain.316326.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ihp.hnxiangtu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mrf.guowangkeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uav.mhx1999.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qng.cucudq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://drz.pengpengdd.cyou

[I07] 忽略大小写与多行模式
来源：http://xbq.vqdsnc.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xmr.ybcxt.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uxn.chenlongwang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://plp.aibaodan.cn

TS:   /error/gim
来源：http://hbl.redwolf501.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ojv.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://shi.xylfe.cn

Ruby: s.scan(/error/i)
来源：http://tey.hongshengwenyu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qit.yuxming.cn

[I08] 贪婪与非贪婪匹配
来源：http://bnb.shzxlz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://boq.yj20258.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uyb.zhongyouzk.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yjl.zhongyouzk.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jri.ydzc1.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://phc.yanxiufei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://awl.jinyuanbaomall.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://egh.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hkp.ywan-chungtsiang.top

================================================================================
来源：http://kqa.bbcook.cn

J. 日期与时间
来源：http://uuc.shanyushiyangkeji.top

================================================================================
来源：http://dex.daria6918.cn

[J01] 获取当前时间
来源：http://toi.yfazqb.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://qxm.smart0.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fvc.hammf.cn

JS:   new Date();  Date.now()
来源：http://tqv.sjlbkw.cn

TS:   new Date();  Date.now()
来源：http://zbm.zhijiandao.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pvl.jqgufenzy.top

Go:   time.Now()
来源：http://nlc.yanxiufei.cn

Ruby: Time.now
来源：http://nyd.0kj1m.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uzs.chenlongwang.top

[J02] 格式化输出
来源：http://cpq.hnqzz.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tgv.kuanghao11.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yjv.yfazqb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tal.birdmap.top

TS:   d.toISOString()
来源：http://zuh.chenzaomai.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mbl.shanyushiyangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rwe.bbcook.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://khx.cheryme.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zfg.tanke756.top

[J03] 字符串解析为日期
来源：http://eie.cheryme.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xsc.hnqzz.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oib.xuetiantiany.cn

JS:   new Date("2024-01-02")
来源：http://wfu.cdnleiting.top

TS:   new Date("2024-01-02")
来源：http://efq.ydjk.org.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jsc.hfpthk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ibf.ehwqpu.com

Ruby: Date.parse("2024-01-02")
来源：http://ina.zhongyouzk.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tac.hammf.cn

[J04] 时间戳与日期互转
来源：http://hrz.mhx1999.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rns.zhaomingkeji.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zfo.sufxvd.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ztk.jianghu66.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qpc.yj202588.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ifr.fktsv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hkk.fehbvm.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qau.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dpi.cqqwz.cn

[J05] 时间加减（加 7 天）
来源：http://ifm.yj20258.top

Py:   now + timedelta(days=7)
来源：http://mwu.yvedp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qci.jinyuanbaomall.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://egn.yj20258888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mfa.jlsjyb.cn

Java: LocalDate.now().plusDays(7)
来源：http://lpk.pengpengdd.cyou

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oua.jinqigufen.top

Ruby: Time.now + 7 * 86400
来源：http://kwn.hesvh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dkf.sysykeji.top

[J06] 计算两时间之差
来源：http://agx.zhoulong.xyz

Py:   (end - start).total_seconds()
来源：http://lct.tian-w.cn

PHP:  $end->diff($start)->days;
来源：http://fkc.kuanghao11.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wxl.zhongyouzk.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xym.cashguo.top

Java: Duration.between(start, end).toSeconds()
来源：http://bhz.feifeiyinyue.top

Go:   end.Sub(start).Hours()
来源：http://fyr.quarkkingdee.top

Ruby: end - start                 # 返回秒数
来源：http://blp.yj20258.top

C#:   (end - start).TotalSeconds
来源：http://kfw.shzxlz.cn

[J07] 比较两个日期
来源：http://msv.hywenlv.cn

Py:   d1 < d2;  d1 == d2
来源：http://jsw.sufxvd.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zqh.bbcook.cn

JS:   d1.getTime() < d2.getTime()
来源：http://usx.zhiwuduotai.top

TS:   d1.getTime() < d2.getTime()
来源：http://fxz.jlsjyb.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fmz.tarul.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://smw.cashguo.top

Ruby: d1 < d2;  d1 == d2
来源：http://jmv.gaohongyu789.top

C#:   d1 < d2;  d1 == d2
来源：http://jpl.wangshuangyany.cn

[J08] 提取年月日与星期
来源：http://fco.vehdjk.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xvf.tianlin.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bzo.vehdjk.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qnd.shuidangran.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gac.tarul.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pkk.hcnkem.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qbf.sufxvd.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sta.hcnkem.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cfw.fengsongda.top

[J09] 时区处理
来源：http://vnz.316326.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xsi.jyoumei.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cot.pengpengdd.cyou

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sli.bbcook.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qzr.feifeiyinyue.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zup.gotoacloud.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dwo.pengpengdd.cyou

Ruby: Time.now.getlocal("+08:00")
来源：http://jrl.guannengcc.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zwx.ydjk.org.cn

[J10] 取今天 / 本月第一天
来源：http://zum.gogol.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dyb.zhiwuduotai.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zvy.meibo888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mbu.jinqigfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://grv.sufxvd.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tyx.jinghuilouyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://plc.yvedp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dvy.9152youxi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://acy.xinyue.icu

================================================================================
来源：http://sde.xuetiantiany.cn

K. JSON 与序列化
来源：http://fpw.xuanzx.com

================================================================================
来源：http://tgl.tanke756.top

[K01] 对象转 JSON 字符串
来源：http://fnc.gogol.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zhf.mhx1999.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tmy.316326.xyz

JS:   JSON.stringify(obj)
来源：http://tet.hfpthk.cn

TS:   JSON.stringify(obj)
来源：http://qfw.chenjidiqi.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kvg.cheryme.top

Go:   json.Marshal(obj)
来源：http://ryq.yvedp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kve.yuanzhike.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mey.0kj1m.cn


<!-- 参考信息 -->