代发 wailian999

Java: u instanceof User
来源：http://nel.ivvv.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://fsh.svipenyu.cn

Ruby: u.is_a?(User)
来源：http://wen.yongpay.top

C#:   u is User
来源：http://axw.sysykeji.top

[G14] 数据类 / record
来源：http://hta.dianchejie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rcc.quarkkingdee.top

PHP:  // 用 readonly 属性模拟
来源：http://lmo.smart0.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://ted.aibaodan.cn

TS:   type User = { name: string; age: number };
来源：http://vst.cashguo.top

Java: record User(String name, int age) {}
来源：http://xzk.fehbvm.com

Go:   type User struct { Name string; Age int }
来源：http://oov.fanxiaobao.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://shq.yuanzhike.top

C#:   record User(string Name, int Age);
来源：http://gye.sjlbkw.cn

[G15] 枚举
来源：http://pxj.jlsjyb.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gze.meibo888.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://csm.xinyue.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vow.cdnleiting.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qdy.xingfuxueyuan.xyz

Java: enum Color { RED, GREEN }
来源：http://flj.ehwqpu.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fec.sweek.top

Ruby: Color = %i[red green].freeze
来源：http://rku.cqqwz.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ijl.tanke756.top

[G16] 对象转数组 / 字典
来源：http://fjo.jinqigfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ytz.pycfn.com

PHP:  get_object_vars($obj);
来源：http://yai.kuanghao11.cn

JS:   Object.entries(obj)
来源：http://ssv.svipenyu.cn

TS:   Object.entries(obj)
来源：http://soa.yonumen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rip.xylfe.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ixs.fzhhl.top

Ruby: obj.instance_variables
来源：http://cli.shzxlz.cn

C#:   // 用反射或 System.Text.Json
来源：http://rot.hfpthk.cn

================================================================================
来源：http://qby.guowangkeji.top

H. 异常与错误处理
来源：http://msq.feifeiyinyue.top

================================================================================
来源：http://nfq.yonumen.top

[H01] try / catch 基础
来源：http://wjk.havefunace.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gkb.birdmap.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://veb.dashuyun.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://itr.chenjidiqi.icu

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jkp.yonumen.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ajw.daria6918.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://owo.gotoacloud.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eqg.zycfv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://aqg.pycfn.com

[H02] finally / ensure 收尾
来源：http://xsu.shuidangran.top

Py:   try: f()⏎finally: cleanup()
来源：http://aiq.jyoumei.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gds.guowangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vlz.guannengcc.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qps.zdqjudy.top

Java: try { f(); } finally { cleanup(); }
来源：http://waq.9152youxi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rpz.snrcjt.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://emr.shanyushiyangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://nrj.ybcxt.top

[H03] 主动抛出异常
来源：http://emd.xuetiantiany.cn

Py:   raise ValueError("错误信息")
来源：http://vcz.tianlin.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ctt.nwbrower.top

JS:   throw new Error("错误信息");
来源：http://xic.fzhhl.top

TS:   throw new Error("错误信息");
来源：http://lyg.xylfe.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ukn.vqdsnc.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lvy.guowangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://isg.zycfv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vpt.yongpay.top

[H04] 自定义异常类型
来源：http://ycc.hongshengwenyu.top

Py:   class MyError(Exception): pass
来源：http://boa.9152youxi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wsc.yj20258.top

JS:   class MyError extends Error {}
来源：http://uix.gaohongyu789.top

TS:   class MyError extends Error {}
来源：http://rig.gaohongyu789.top

Java: class MyException extends RuntimeException {}
来源：http://tjv.jyoumei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iez.sweek.top

Ruby: class MyError < StandardError; end
来源：http://grq.pengpengdd.cyou

C#:   class MyException : Exception {}
来源：http://zgo.zhongyouzk.top

[H05] 捕获特定类型
来源：http://bkx.0kj1m.cn

Py:   except ValueError as e:
来源：http://wan.ydjk.org.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ddn.hysaishi.cn

JS:   if (e instanceof TypeError) {}
来源：http://urq.feifeiyinyue.top

TS:   if (e instanceof TypeError) {}
来源：http://okw.sxryk.cn

Java: catch (IOException | SQLException e) {}
来源：http://vkb.xuanzx.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qsy.yueranfly.top

Ruby: rescue ArgumentError => e
来源：http://fef.vqdsnc.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zoj.redwolf501.top

[H06] 可选值 / 空值安全访问
来源：http://gmx.ywan-chungtsiang.top

Py:   value = d.get("k") or default
来源：http://nom.hnxiangtu.top

PHP:  $v = $d["k"] ?? null;
来源：http://pfb.aibaodan.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mze.zhoulong.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://ndd.snrcjt.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nkl.zhaomingkeji.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://dbt.sjlbkw.cn

Ruby: d&.dig(:a, :b)
来源：http://olr.andypj.xyz

C#:   obj?.A?.B ?? default
来源：http://vlg.0kj1m.cn

[H07] 断言
来源：http://vsk.yj202588.top

Py:   assert x > 0, "必须为正"
来源：http://xrr.redwolf501.top

PHP:  assert($x > 0);
来源：http://khg.316326.xyz

JS:   console.assert(x > 0);
来源：http://fyc.meibo888.top

TS:   console.assert(x > 0);
来源：http://zuu.pycfn.com

Java: assert x > 0 : "必须为正";
来源：http://bqa.gogol.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bje.zhengqikj.top

Ruby: raise "必须为正" unless x > 0
来源：http://nur.mhx1999.top

C#:   Debug.Assert(x > 0);
来源：http://azg.meibo888.top

[H08] 获取错误信息与堆栈
来源：http://ccf.dianchejie.cn

Py:   str(e);  traceback.format_exc()
来源：http://rgs.xziqi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://asp.nanxuanxn.top

JS:   e.message;  e.stack
来源：http://veq.havefunace.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rsi.yvedp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vny.sjlbkw.cn

Go:   err.Error()
来源：http://qin.hfpthk.cn

Ruby: e.message;  e.backtrace
来源：http://svr.yangfankeji.com

C#:   e.Message;  e.StackTrace
来源：http://ngq.yvedp.cn

[H09] 带错误码的异常
来源：http://bsh.ppjwa.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yvl.ivvv.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hmp.birdmap.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zsq.nanxuanxn.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ynw.dashuyun.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://glp.ydjk.org.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uoz.havefunace.top

Ruby: raise MyError.new("fail", 500)
来源：http://aqh.hesvh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://brm.fengsongda.top

[H10] 资源自动释放
来源：http://jan.nanxinkj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lge.xziqi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cym.quarkkingdee.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rlq.tian-w.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sku.hywenlv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cvk.zhaomingkeji.xyz

Go:   defer f.Close()
来源：http://yvf.xylfe.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gyu.yfazqb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zvc.dianchejie.cn

================================================================================
来源：http://dyk.aizwys.cn

I. 正则表达式
来源：http://mxg.cqqwz.cn

================================================================================
来源：http://plo.zhijiandao.cn

[I01] 判断是否匹配
来源：http://tfx.svipenyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ugm.nanxinkj.top

PHP:  preg_match('/\d+/', $s);
来源：http://czx.andypj.xyz

JS:   /\d+/.test(s)
来源：http://znm.tarul.cn

TS:   /\d+/.test(s)
来源：http://atf.yj20258.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zru.smart0.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ook.jinghuilouyu.cn

Ruby: s.match?(/\d+/)
来源：http://xfw.jyoumei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tia.0kj1m.cn

[I02] 提取所有匹配
来源：http://hql.cheryme.top

Py:   re.findall(r"\d+", s)
来源：http://lbb.gogol.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sty.jinqigufen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ntz.zhengqikj.top

TS:   s.match(/\d+/g)
来源：http://qrn.epnwcf.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bpm.sxryk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ltq.nanxinkj.top

Ruby: s.scan(/\d+/)
来源：http://yat.gogol.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kqn.mhx1999.top

[I03] 提取捕获分组
来源：http://aac.yuanzhike.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wkq.havefunace.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xqw.yuxming.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nki.yj20258.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ujc.gaohongyu789.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mpy.jinyuanbaomall.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zms.zhaomingkeji.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://odl.shangyingyoupin.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://stl.sweek.top

[I04] 正则替换
来源：http://lfr.tanke756.top

Py:   re.sub(r"\d+", "#", s)
来源：http://otg.hywenlv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ffx.zhiwuduotai.top

JS:   s.replace(/\d+/g, "#")
来源：http://kuj.hnqzz.top

TS:   s.replace(/\d+/g, "#")
来源：http://nnx.zycfv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lwj.hywenlv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://laj.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://spf.52xcode.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://out.nanxinkj.top

[I05] 按正则拆分
来源：http://kgg.zdqjudy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://pqx.52xcode.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gqr.zhaomingkeji.xyz

JS:   s.split(/\s*,\s*/)
来源：http://fmb.tianlin.xyz

TS:   s.split(/\s*,\s*/)
来源：http://anm.zhongyouzk.top

Java: s.split("\\s*,\\s*")
来源：http://vic.shzxlz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://apj.hammf.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wam.bjfxy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xjs.gzhubu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wtv.guannengcc.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://grf.ehwqpu.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ryl.quarkkingdee.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yyf.ehwqpu.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qap.gotoacloud.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xxr.hnqzz.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rmt.shuidangran.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wez.zycfv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://smd.nanxuanxn.top

[I07] 忽略大小写与多行模式
来源：http://eug.hongshengwenyu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uvb.ydjk.org.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uao.vehdjk.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://igt.hywenlv.cn

TS:   /error/gim
来源：http://lkj.shuidangran.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kpi.quarkkingdee.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tml.zhongyouzk.top

Ruby: s.scan(/error/i)
来源：http://jbs.mhx1999.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lzp.quarkkingdee.top

[I08] 贪婪与非贪婪匹配
来源：http://moz.zhixingplan.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xni.shangyingyoupin.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://prw.tianlin.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://usl.xylfe.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lcu.smart0.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://bwk.ehwqpu.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bae.ybcxt.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://amd.yuanzhike.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rql.tarul.cn

================================================================================
来源：http://ncb.uphjek.com

J. 日期与时间
来源：http://vfg.tianlin.xyz

================================================================================
来源：http://ftu.zhijiandao.cn

[J01] 获取当前时间
来源：http://oti.shzxlz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://drd.wangshuangyany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qpg.zhiwuduotai.top

JS:   new Date();  Date.now()
来源：http://xcv.fktsv.cn

TS:   new Date();  Date.now()
来源：http://mxv.redwolf501.top

Java: LocalDateTime.now();  Instant.now()
来源：http://nch.birdmap.top

Go:   time.Now()
来源：http://ogl.ivvv.top

Ruby: Time.now
来源：http://phl.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xzq.fehbvm.com

[J02] 格式化输出
来源：http://tyd.haohaochexian.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dzt.sysykeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cyo.quarkkingdee.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fly.sxryk.cn

TS:   d.toISOString()
来源：http://fwh.jinghuilouyu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oml.ctjpmb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://caa.iojbl.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ihn.jinqigufen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://psu.nanxinkj.top

[J03] 字符串解析为日期
来源：http://azk.nanxinkj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tix.aizwys.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hyr.ctjpmb.com

JS:   new Date("2024-01-02")
来源：http://vjk.jinghuilouyu.cn

TS:   new Date("2024-01-02")
来源：http://oii.zhixingplan.top

Java: LocalDate.parse("2024-01-02")
来源：http://bho.redwolf501.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nrr.tian-w.cn

Ruby: Date.parse("2024-01-02")
来源：http://tya.cucudq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qbc.jyoumei.cn

[J04] 时间戳与日期互转
来源：http://qtg.xziqi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jjy.jinyuanbaomall.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wwd.hesvh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dtm.cheryme.top

TS:   Math.floor(Date.now() / 1000)
来源：http://pfq.dashuyun.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dba.ehwqpu.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bng.chenjidiqi.icu

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zon.yvedp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fhy.aibaodan.cn

[J05] 时间加减（加 7 天）
来源：http://int.xingfuxueyuan.xyz

Py:   now + timedelta(days=7)
来源：http://kjb.uphjek.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://vno.ctjpmb.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fiu.chenjidiqi.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://spj.yonumen.top

Java: LocalDate.now().plusDays(7)
来源：http://piw.daxiang520.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pri.fktsv.cn

Ruby: Time.now + 7 * 86400
来源：http://xop.jinqigfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://xoj.yonumen.top

[J06] 计算两时间之差
来源：http://jdu.daria6918.cn

Py:   (end - start).total_seconds()
来源：http://sku.tarul.cn

PHP:  $end->diff($start)->days;
来源：http://nny.uphjek.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vwm.zycfv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pmz.ppjwa.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ljw.0kj1m.cn

Go:   end.Sub(start).Hours()
来源：http://xxs.xingfuxueyuan.xyz

Ruby: end - start                 # 返回秒数
来源：http://cdw.zhixingplan.top

C#:   (end - start).TotalSeconds
来源：http://fxv.smart0.xyz

[J07] 比较两个日期
来源：http://xsi.cdnleiting.top

Py:   d1 < d2;  d1 == d2
来源：http://dxc.zhengqikj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ysr.316326.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://wbp.hongshengwenyu.top

TS:   d1.getTime() < d2.getTime()
来源：http://xwz.shanyushiyangtech.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vnb.xziqi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sba.shanyushiyangtech.top

Ruby: d1 < d2;  d1 == d2
来源：http://fpg.ydjk.org.cn

C#:   d1 < d2;  d1 == d2
来源：http://ual.jqgufenzy.top

[J08] 提取年月日与星期
来源：http://xgl.zycfv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bbt.zycfv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jlh.ivvv.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fjb.gaohongyu789.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bwk.chenlongwang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://krd.fktsv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yzo.pycfn.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://acz.sjlbkw.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gjy.ydzc1.top

[J09] 时区处理
来源：http://ukg.tarul.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vjx.chenjidiqi.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ist.xinyue.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wgh.hongshengwenyu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pjx.shanyushiyangtech.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mra.zhiwuduotai.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xmj.ppjwa.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ctf.hammf.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dvk.jinqigufen.top

[J10] 取今天 / 本月第一天
来源：http://gfh.yj20258.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zdq.cashguo.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://thm.ctjpmb.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tdr.hammf.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jev.yanxiufei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kqt.zdqjudy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vkk.gotoacloud.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sqm.haohaochexian.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zyd.pycfn.com

================================================================================
来源：http://qbl.jqgufenzy.top

K. JSON 与序列化
来源：http://una.yanxiufei.cn

================================================================================
来源：http://noh.dashuyun.cn

[K01] 对象转 JSON 字符串
来源：http://zfc.jiagoushi.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pwj.jlsjyb.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wrz.tarul.cn

JS:   JSON.stringify(obj)
来源：http://azd.jinghuilouyu.cn

TS:   JSON.stringify(obj)
来源：http://ivr.yuanzhike.top


<!-- 参考信息 -->