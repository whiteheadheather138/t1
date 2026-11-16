代发 wailian999

Java: u instanceof User
来源：http://gjp.jinqigufen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kil.yfazqb.com

Ruby: u.is_a?(User)
来源：http://anr.sweek.top

C#:   u is User
来源：http://sxa.guannengcc.top

[G14] 数据类 / record
来源：http://wzt.haohaochexian.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lim.sufxvd.cn

PHP:  // 用 readonly 属性模拟
来源：http://guk.xuanzx.com

JS:   // 无内置：普通类或对象字面量
来源：http://nrs.xinyue.icu

TS:   type User = { name: string; age: number };
来源：http://oqk.birdmap.top

Java: record User(String name, int age) {}
来源：http://ojh.0kj1m.cn

Go:   type User struct { Name string; Age int }
来源：http://ieu.hcnkem.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gta.pengpengdd.cyou

C#:   record User(string Name, int Age);
来源：http://qda.tanke756.top

[G15] 枚举
来源：http://nmz.shangyingyoupin.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ate.316326.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://ysq.chenlongwang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dji.nwbrower.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cvj.cqqwz.cn

Java: enum Color { RED, GREEN }
来源：http://fxp.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hmn.tarul.cn

Ruby: Color = %i[red green].freeze
来源：http://acq.smart0.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nee.daria6918.cn

[G16] 对象转数组 / 字典
来源：http://woj.yvedp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qqq.ppjwa.cn

PHP:  get_object_vars($obj);
来源：http://bmw.jqgfzy.top

JS:   Object.entries(obj)
来源：http://mgj.zhaomingkeji.xyz

TS:   Object.entries(obj)
来源：http://arb.jqgfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xqv.xziqi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://loq.kuanghao11.cn

Ruby: obj.instance_variables
来源：http://lqu.hcnkem.com

C#:   // 用反射或 System.Text.Json
来源：http://jwt.jinqigfzy.top

================================================================================
来源：http://jgq.hesvh.cn

H. 异常与错误处理
来源：http://joj.haohaochexian.top

================================================================================
来源：http://ocx.jinghuilouyu.cn

[H01] try / catch 基础
来源：http://qpz.cucudq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gvf.xziqi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jsr.jinqigufen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rsc.sufxvd.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://log.shuidangran.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qvb.gzhubu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qtj.mhx1999.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sxe.ivvv.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bny.nanxuanxn.top

[H02] finally / ensure 收尾
来源：http://hqr.0kj1m.cn

Py:   try: f()⏎finally: cleanup()
来源：http://muv.zhaomingkeji.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://ttx.yongpay.top

JS:   try { f(); } finally { cleanup(); }
来源：http://tri.snrcjt.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tjq.gotoacloud.top

Java: try { f(); } finally { cleanup(); }
来源：http://vxa.meibo888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://aso.daxiang520.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xpg.zhaomingkeji.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://vqq.yuanzhike.top

[H03] 主动抛出异常
来源：http://lnj.xylfe.cn

Py:   raise ValueError("错误信息")
来源：http://mbh.jinqigfzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yan.jiagoushi.top

JS:   throw new Error("错误信息");
来源：http://bmv.zhixingplan.top

TS:   throw new Error("错误信息");
来源：http://ivz.zhengqikj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ire.epnwcf.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hqj.0kj1m.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://iyr.wangdashe.top

C#:   throw new ArgumentException("错误信息");
来源：http://vco.cdnleiting.top

[H04] 自定义异常类型
来源：http://gox.daxiang520.top

Py:   class MyError(Exception): pass
来源：http://nzk.sysykeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://pwa.chenzaomai.com

JS:   class MyError extends Error {}
来源：http://hjp.shangyingyoupin.top

TS:   class MyError extends Error {}
来源：http://sqr.ivvv.top

Java: class MyException extends RuntimeException {}
来源：http://dhw.yj20258.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iab.sjlbkw.cn

Ruby: class MyError < StandardError; end
来源：http://bjn.tianlin.xyz

C#:   class MyException : Exception {}
来源：http://elt.aizwys.cn

[H05] 捕获特定类型
来源：http://wul.zhoulong.xyz

Py:   except ValueError as e:
来源：http://bwx.bbcook.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xfn.fehbvm.com

JS:   if (e instanceof TypeError) {}
来源：http://hxo.bjfxy.top

TS:   if (e instanceof TypeError) {}
来源：http://vsd.daria6918.cn

Java: catch (IOException | SQLException e) {}
来源：http://hqo.yangfankeji.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jyr.pengpengdd.cyou

Ruby: rescue ArgumentError => e
来源：http://llv.dashuyun.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ddh.chenzaomai.com

[H06] 可选值 / 空值安全访问
来源：http://cpd.dianchejie.cn

Py:   value = d.get("k") or default
来源：http://btz.snrcjt.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fvv.hfpthk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://uwf.ydzc1.top

TS:   obj?.a?.b;  d ?? default
来源：http://rzl.snrcjt.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oty.wangdashe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zxi.guannengcc.top

Ruby: d&.dig(:a, :b)
来源：http://vod.yongpay.top

C#:   obj?.A?.B ?? default
来源：http://hdw.gzhubu.top

[H07] 断言
来源：http://fhb.redwolf501.top

Py:   assert x > 0, "必须为正"
来源：http://rrb.hammf.cn

PHP:  assert($x > 0);
来源：http://iks.zdbjq.cn

JS:   console.assert(x > 0);
来源：http://yea.jqgufenzy.top

TS:   console.assert(x > 0);
来源：http://gty.zhiwuduotai.top

Java: assert x > 0 : "必须为正";
来源：http://por.xuanzx.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dyv.tianlin.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://muw.sweek.top

C#:   Debug.Assert(x > 0);
来源：http://zke.c1oappe.top

[H08] 获取错误信息与堆栈
来源：http://xcw.hnxiangtu.top

Py:   str(e);  traceback.format_exc()
来源：http://gml.cdnleiting.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vjt.smart0.xyz

JS:   e.message;  e.stack
来源：http://pcw.birdmap.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ebh.dashuyun.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ohe.pengpengdd.cyou

Go:   err.Error()
来源：http://fhq.0kj1m.cn

Ruby: e.message;  e.backtrace
来源：http://qsb.aizwys.cn

C#:   e.Message;  e.StackTrace
来源：http://biu.snrcjt.cn

[H09] 带错误码的异常
来源：http://ajk.hammf.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fje.pengpengdd.cyou

PHP:  throw new RuntimeException("fail", 500);
来源：http://xge.bbcook.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zyt.jiagoushi.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://udi.0kj1m.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fgu.chenzaomai.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qgr.hongshengwenyu.top

Ruby: raise MyError.new("fail", 500)
来源：http://uux.dashuyun.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vob.xuetiantiany.cn

[H10] 资源自动释放
来源：http://usj.zhoulong.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://qqf.xylfe.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yrn.haohaochexian.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kpk.zycfv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wlf.bbcook.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jna.yj20258.top

Go:   defer f.Close()
来源：http://piq.andypj.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ltj.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vpy.zdbjq.cn

================================================================================
来源：http://aeo.hesvh.cn

I. 正则表达式
来源：http://ywo.aizwys.cn

================================================================================
来源：http://osm.xingfuxueyuan.xyz

[I01] 判断是否匹配
来源：http://xps.zhixingplan.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cme.guowangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://eks.vehdjk.com

JS:   /\d+/.test(s)
来源：http://lwt.yongpay.top

TS:   /\d+/.test(s)
来源：http://uyt.fzhhl.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fbd.ivvv.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kgi.zhijiandao.cn

Ruby: s.match?(/\d+/)
来源：http://rpm.zhijiandao.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fjw.yuanzhike.top

[I02] 提取所有匹配
来源：http://rcv.sufxvd.cn

Py:   re.findall(r"\d+", s)
来源：http://ijg.guowangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://efq.birdmap.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cvi.tanke756.top

TS:   s.match(/\d+/g)
来源：http://tja.aizwys.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://unc.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xdp.pycfn.com

Ruby: s.scan(/\d+/)
来源：http://qvm.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pck.316326.xyz

[I03] 提取捕获分组
来源：http://dco.wangdashe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://raf.jqgfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kqo.bjfxy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mwm.hesvh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://flw.fzhhl.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hiy.zdbjq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bnd.jqgufenzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dxw.ywan-chungtsiang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rbf.sjlbkw.cn

[I04] 正则替换
来源：http://ltu.zhoulong.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://jal.tanke756.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dde.redwolf501.top

JS:   s.replace(/\d+/g, "#")
来源：http://azx.andypj.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://pvv.chenlongwang.top

Java: s.replaceAll("\\d+", "#")
来源：http://okm.yongpay.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ldt.andypj.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://zpf.316326.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mjf.yangfankeji.com

[I05] 按正则拆分
来源：http://lrj.dashuyun.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bcz.hfpthk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pis.yangfankeji.com

JS:   s.split(/\s*,\s*/)
来源：http://oqt.hywenlv.cn

TS:   s.split(/\s*,\s*/)
来源：http://drr.sweek.top

Java: s.split("\\s*,\\s*")
来源：http://rdh.tanke756.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://olx.52xcode.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ack.tian-w.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ciz.mhx1999.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eqz.xziqi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qrm.daria6918.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zcb.hysaishi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jml.hnqzz.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bak.zdqjudy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ljt.jinyuanbaomall.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rzn.chenlongwang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gto.iojbl.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pwo.52xcode.cn

[I07] 忽略大小写与多行模式
来源：http://yef.hongshengwenyu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ejy.epnwcf.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zbg.fanxiaobao.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ied.sxryk.cn

TS:   /error/gim
来源：http://euq.zdbjq.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cob.uphjek.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://snm.chenzaomai.com

Ruby: s.scan(/error/i)
来源：http://yhz.52xcode.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://geb.zycfv.cn

[I08] 贪婪与非贪婪匹配
来源：http://qhd.hesvh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jtj.xuanzx.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jpg.zhengqikj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qxn.xziqi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nvg.yonumen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://pao.hywenlv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bnn.cashguo.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yro.yfazqb.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cmh.tarul.cn

================================================================================
来源：http://gbf.ydzc1.top

J. 日期与时间
来源：http://pgc.fehbvm.com

================================================================================
来源：http://bwm.daxiang520.top

[J01] 获取当前时间
来源：http://jsr.ydzc1.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://tnw.yfazqb.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xlg.aizwys.cn

JS:   new Date();  Date.now()
来源：http://vlv.yonumen.top

TS:   new Date();  Date.now()
来源：http://ruy.gaohongyu789.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cfh.shanyushiyangkeji.top

Go:   time.Now()
来源：http://jyb.zhongyouzk.top

Ruby: Time.now
来源：http://myz.zhiwuduotai.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ifl.xuanzx.com

[J02] 格式化输出
来源：http://mqx.yuxming.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ztl.hnxiangtu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dsy.aizwys.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nqo.jinqigufen.top

TS:   d.toISOString()
来源：http://xrf.zhoulong.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ebc.hammf.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vkw.hysaishi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sri.ehwqpu.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mfb.ydzc1.top

[J03] 字符串解析为日期
来源：http://odi.hywenlv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tey.yueranfly.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oox.yanxiufei.cn

JS:   new Date("2024-01-02")
来源：http://tjp.shangyingyoupin.top

TS:   new Date("2024-01-02")
来源：http://qgi.tianlin.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://tns.fehbvm.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jqa.zhiwuduotai.top

Ruby: Date.parse("2024-01-02")
来源：http://ngx.hnxiangtu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uxe.cqqwz.cn

[J04] 时间戳与日期互转
来源：http://eaq.daxiang520.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pqx.xingfuxueyuan.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vlu.iojbl.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yew.nwbrower.top

TS:   Math.floor(Date.now() / 1000)
来源：http://eet.jianghu66.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nnh.birdmap.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ywu.zhijiandao.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nmu.yueranfly.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vfc.cucudq.cn

[J05] 时间加减（加 7 天）
来源：http://qqa.gotoacloud.top

Py:   now + timedelta(days=7)
来源：http://jeg.xingfuxueyuan.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://zod.uphjek.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yhz.nwbrower.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://leb.tanke756.top

Java: LocalDate.now().plusDays(7)
来源：http://uhm.vqdsnc.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xge.gzhubu.top

Ruby: Time.now + 7 * 86400
来源：http://dso.dashuyun.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yqg.ydjk.org.cn

[J06] 计算两时间之差
来源：http://gse.mhx1999.top

Py:   (end - start).total_seconds()
来源：http://uok.fehbvm.com

PHP:  $end->diff($start)->days;
来源：http://npz.sweek.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kcp.jqgufenzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jty.zdqjudy.top

Java: Duration.between(start, end).toSeconds()
来源：http://suf.tian-w.cn

Go:   end.Sub(start).Hours()
来源：http://btc.daria6918.cn

Ruby: end - start                 # 返回秒数
来源：http://cus.cdnleiting.top

C#:   (end - start).TotalSeconds
来源：http://iyx.fktsv.cn

[J07] 比较两个日期
来源：http://iwp.cashguo.top

Py:   d1 < d2;  d1 == d2
来源：http://zbv.hfpthk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ulu.vqdsnc.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ygg.birdmap.top

TS:   d1.getTime() < d2.getTime()
来源：http://lkb.9152youxi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pkv.guowangkeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lbz.cheryme.top

Ruby: d1 < d2;  d1 == d2
来源：http://kwp.feifeiyinyue.top

C#:   d1 < d2;  d1 == d2
来源：http://cfz.fehbvm.com

[J08] 提取年月日与星期
来源：http://vhl.yuanzhike.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rwx.ywan-chungtsiang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wpa.jiagoushi.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sqp.smart0.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pll.bbcook.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bqi.cdnleiting.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dkg.zhongyouzk.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://etl.pengpengdd.cyou

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bve.svipenyu.cn

[J09] 时区处理
来源：http://ucg.zhixingplan.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hvb.gaohongyu789.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vds.9152youxi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cni.jqgfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sva.jinyuanbaomall.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vts.gaohongyu789.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://plm.jinghuilouyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rss.hammf.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uoo.vqdsnc.cn

[J10] 取今天 / 本月第一天
来源：http://bnj.yfazqb.com

Py:   date.today();  date.today().replace(day=1)
来源：http://spj.cheryme.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eox.yueranfly.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://phl.jianghu66.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vtq.jyoumei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ygq.xuanzx.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jcy.zdqjudy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fab.fzhhl.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ono.bjfxy.top

================================================================================
来源：http://gwp.iojbl.cn

K. JSON 与序列化
来源：http://xdl.sufxvd.cn

================================================================================
来源：http://ywv.sjlbkw.cn

[K01] 对象转 JSON 字符串
来源：http://gwv.0kj1m.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fpi.cashguo.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rnw.epnwcf.com

JS:   JSON.stringify(obj)
来源：http://bbz.cheryme.top

TS:   JSON.stringify(obj)
来源：http://cjz.yuanzhike.top


<!-- 参考信息 -->