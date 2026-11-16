代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://evt.yj20258.top

Ruby: def to_s; @name; end
来源：http://tcj.yuanzhike.top

C#:   public override string ToString() => Name;
来源：http://ddb.quarkkingdee.top

[G13] 判断对象类型
来源：http://lyt.fehbvm.com

Py:   isinstance(u, User)
来源：http://jmy.kuanghao11.cn

PHP:  $u instanceof User
来源：http://kdm.cashguo.top

JS:   u instanceof User
来源：http://yit.haohaochexian.top

TS:   u instanceof User
来源：http://fog.ctjpmb.com

Java: u instanceof User
来源：http://pij.shanyushiyangtech.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://npq.epnwcf.com

Ruby: u.is_a?(User)
来源：http://cag.316326.xyz

C#:   u is User
来源：http://hab.quarkkingdee.top

[G14] 数据类 / record
来源：http://zek.shanyushiyangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iob.vehdjk.com

PHP:  // 用 readonly 属性模拟
来源：http://fpr.zhixingplan.top

JS:   // 无内置：普通类或对象字面量
来源：http://owh.yongpay.top

TS:   type User = { name: string; age: number };
来源：http://cun.zhongyouzk.top

Java: record User(String name, int age) {}
来源：http://wxf.ppjwa.cn

Go:   type User struct { Name string; Age int }
来源：http://qfg.cdnleiting.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xjd.fanxiaobao.xyz

C#:   record User(string Name, int Age);
来源：http://qiu.yj20258888.top

[G15] 枚举
来源：http://tsi.nwbrower.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fdl.sxryk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nxd.xylfe.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qou.zhoulong.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tjd.vqdsnc.cn

Java: enum Color { RED, GREEN }
来源：http://yau.pycfn.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uyf.jianghu66.top

Ruby: Color = %i[red green].freeze
来源：http://dyr.fanxiaobao.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vum.guannengcc.top

[G16] 对象转数组 / 字典
来源：http://qhp.uphjek.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tig.haohaochexian.top

PHP:  get_object_vars($obj);
来源：http://wxb.pengpengdd.cyou

JS:   Object.entries(obj)
来源：http://qzm.zdqjudy.top

TS:   Object.entries(obj)
来源：http://mzh.tanke756.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yjx.nwbrower.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xwz.guannengcc.top

Ruby: obj.instance_variables
来源：http://yrc.sxryk.cn

C#:   // 用反射或 System.Text.Json
来源：http://bbn.zhengqikj.top

================================================================================
来源：http://twq.zhiwuduotai.top

H. 异常与错误处理
来源：http://bok.zhaomingkeji.xyz

================================================================================
来源：http://lfu.feifeiyinyue.top

[H01] try / catch 基础
来源：http://uef.gogol.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yzc.xuetiantiany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hys.svipenyu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qxg.jinghuilouyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hgb.hysaishi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lum.tarul.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cee.ivvv.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pgw.jlsjyb.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pfa.hysaishi.cn

[H02] finally / ensure 收尾
来源：http://uws.hnxiangtu.top

Py:   try: f()⏎finally: cleanup()
来源：http://xkz.bbcook.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yhj.aibaodan.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jci.ivvv.top

TS:   try { f(); } finally { cleanup(); }
来源：http://phg.xinyue.icu

Java: try { f(); } finally { cleanup(); }
来源：http://jzl.ehwqpu.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://ykt.9152youxi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fby.xinyue.icu

C#:   try { F(); } finally { Cleanup(); }
来源：http://glw.zdbjq.cn

[H03] 主动抛出异常
来源：http://qoh.tanke756.top

Py:   raise ValueError("错误信息")
来源：http://rvo.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mjd.yanxiufei.cn

JS:   throw new Error("错误信息");
来源：http://cvn.tianlin.xyz

TS:   throw new Error("错误信息");
来源：http://udq.dashuyun.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://etp.9152youxi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nrz.xingfuxueyuan.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://vdd.yj20258888.top

C#:   throw new ArgumentException("错误信息");
来源：http://zmw.yanxiufei.cn

[H04] 自定义异常类型
来源：http://vrq.hongshengwenyu.top

Py:   class MyError(Exception): pass
来源：http://yge.gzhubu.top

PHP:  class MyError extends RuntimeException {}
来源：http://zeo.tanke756.top

JS:   class MyError extends Error {}
来源：http://rdl.9152youxi.cn

TS:   class MyError extends Error {}
来源：http://ahz.sweek.top

Java: class MyException extends RuntimeException {}
来源：http://izs.uphjek.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rxp.fzhhl.top

Ruby: class MyError < StandardError; end
来源：http://qpo.kuanghao11.cn

C#:   class MyException : Exception {}
来源：http://ewi.xingfuxueyuan.xyz

[H05] 捕获特定类型
来源：http://cai.xuetiantiany.cn

Py:   except ValueError as e:
来源：http://wll.yanxiufei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://osm.zhengqikj.top

JS:   if (e instanceof TypeError) {}
来源：http://dfj.zhoulong.xyz

TS:   if (e instanceof TypeError) {}
来源：http://dck.9152youxi.cn

Java: catch (IOException | SQLException e) {}
来源：http://trx.xziqi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nik.shuidangran.top

Ruby: rescue ArgumentError => e
来源：http://dnl.jinqigufen.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cgu.ybcxt.top

[H06] 可选值 / 空值安全访问
来源：http://sur.yongpay.top

Py:   value = d.get("k") or default
来源：http://ykg.hongshengwenyu.top

PHP:  $v = $d["k"] ?? null;
来源：http://via.wangdashe.top

JS:   obj?.a?.b;  d ?? default
来源：http://clk.sysykeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://kkj.ybcxt.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dpb.daxiang520.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xac.xylfe.cn

Ruby: d&.dig(:a, :b)
来源：http://aeo.tian-w.cn

C#:   obj?.A?.B ?? default
来源：http://psd.ydzc1.top

[H07] 断言
来源：http://gdi.haohaochexian.top

Py:   assert x > 0, "必须为正"
来源：http://mnc.ctjpmb.com

PHP:  assert($x > 0);
来源：http://rsx.chenzaomai.com

JS:   console.assert(x > 0);
来源：http://nxk.0kj1m.cn

TS:   console.assert(x > 0);
来源：http://jcp.chenlongwang.top

Java: assert x > 0 : "必须为正";
来源：http://bed.sufxvd.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fpa.hammf.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pkq.9152youxi.cn

C#:   Debug.Assert(x > 0);
来源：http://vru.yangfankeji.com

[H08] 获取错误信息与堆栈
来源：http://cps.hongshengwenyu.top

Py:   str(e);  traceback.format_exc()
来源：http://qoe.uphjek.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ftq.pycfn.com

JS:   e.message;  e.stack
来源：http://oiy.yuxming.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wfx.yongpay.top

Java: e.getMessage();  e.printStackTrace()
来源：http://okv.cdnleiting.top

Go:   err.Error()
来源：http://tlr.jinqigfzy.top

Ruby: e.message;  e.backtrace
来源：http://srx.ppjwa.cn

C#:   e.Message;  e.StackTrace
来源：http://fau.jinqigufen.top

[H09] 带错误码的异常
来源：http://qbh.tarul.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hmy.jinqigufen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mca.xziqi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kcs.hammf.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ccx.jiagoushi.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jyh.shzxlz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://prt.hammf.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gxe.fengsongda.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gsr.fzhhl.top

[H10] 资源自动释放
来源：http://xwo.fzhhl.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mze.guowangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rzp.xingfuxueyuan.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ysj.vehdjk.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qey.yueranfly.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nrg.ydzc1.top

Go:   defer f.Close()
来源：http://qql.vehdjk.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vmo.chenjidiqi.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rrr.jlsjyb.cn

================================================================================
来源：http://xhm.wangdashe.top

I. 正则表达式
来源：http://ces.hnxiangtu.top

================================================================================
来源：http://peg.cashguo.top

[I01] 判断是否匹配
来源：http://qze.fanxiaobao.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blr.zdbjq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pag.svipenyu.cn

JS:   /\d+/.test(s)
来源：http://jka.hywenlv.cn

TS:   /\d+/.test(s)
来源：http://tjq.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vev.ydjk.org.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jhk.feifeiyinyue.top

Ruby: s.match?(/\d+/)
来源：http://zlf.jianghu66.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rit.yuxming.cn

[I02] 提取所有匹配
来源：http://xpt.ivvv.top

Py:   re.findall(r"\d+", s)
来源：http://wxg.pycfn.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zmk.jqgufenzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ltj.fehbvm.com

TS:   s.match(/\d+/g)
来源：http://kkc.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cmo.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ikm.uphjek.com

Ruby: s.scan(/\d+/)
来源：http://dhb.cdnleiting.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zhs.sufxvd.cn

[I03] 提取捕获分组
来源：http://fci.aibaodan.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lds.snrcjt.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ysa.ctjpmb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iov.yfazqb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://psa.tian-w.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fjt.yongpay.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xzw.yongpay.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mvq.yfazqb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nyi.feifeiyinyue.top

[I04] 正则替换
来源：http://izq.bjfxy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ygx.jiagoushi.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eul.yj202588.top

JS:   s.replace(/\d+/g, "#")
来源：http://zaq.sxryk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nee.haohaochexian.top

Java: s.replaceAll("\\d+", "#")
来源：http://myz.hnxiangtu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vua.hesvh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jfr.uphjek.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pul.ybcxt.top

[I05] 按正则拆分
来源：http://mtu.aibaodan.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pqf.yuanzhike.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xpz.sweek.top

JS:   s.split(/\s*,\s*/)
来源：http://yop.zycfv.cn

TS:   s.split(/\s*,\s*/)
来源：http://kiz.yvedp.cn

Java: s.split("\\s*,\\s*")
来源：http://gsh.cucudq.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uzl.zhaomingkeji.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://hgk.aizwys.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tkb.daxiang520.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tkj.redwolf501.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iig.feifeiyinyue.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gwd.zdbjq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qzs.fengsongda.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://loe.yangfankeji.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://drg.zhixingplan.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zul.kuanghao11.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dsv.ybcxt.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iki.shzxlz.cn

[I07] 忽略大小写与多行模式
来源：http://bgh.aibaodan.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ivo.yueranfly.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vzr.yonumen.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wlq.shuidangran.top

TS:   /error/gim
来源：http://bbl.nanxinkj.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cgq.gzhubu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kjr.ctjpmb.com

Ruby: s.scan(/error/i)
来源：http://int.wangdashe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://azy.shanyushiyangkeji.top

[I08] 贪婪与非贪婪匹配
来源：http://dcj.vehdjk.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zlo.yueranfly.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lzb.wangdashe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hyr.fanxiaobao.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vda.ctjpmb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://qws.ybcxt.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fzz.svipenyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wwe.ivvv.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kpy.zhoulong.xyz

================================================================================
来源：http://znr.nanxuanxn.top

J. 日期与时间
来源：http://mza.fengsongda.top

================================================================================
来源：http://mwl.yonumen.top

[J01] 获取当前时间
来源：http://zhg.yj202588.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wmw.quarkkingdee.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uta.yj20258888.top

JS:   new Date();  Date.now()
来源：http://jfv.zhixingplan.top

TS:   new Date();  Date.now()
来源：http://mnr.jinqigufen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ugb.jyoumei.cn

Go:   time.Now()
来源：http://ahn.c1oappe.top

Ruby: Time.now
来源：http://dht.gzhubu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kej.fehbvm.com

[J02] 格式化输出
来源：http://qoz.shangyingyoupin.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://knj.feifeiyinyue.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pmn.xinyue.icu

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ude.tarul.cn

TS:   d.toISOString()
来源：http://mdb.zhijiandao.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sdr.iojbl.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nfg.ydzc1.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ilb.yuanzhike.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vnp.tanke756.top

[J03] 字符串解析为日期
来源：http://ntw.yongpay.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ptm.jyoumei.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lkb.havefunace.top

JS:   new Date("2024-01-02")
来源：http://mgp.fehbvm.com

TS:   new Date("2024-01-02")
来源：http://mxp.sweek.top

Java: LocalDate.parse("2024-01-02")
来源：http://psc.xylfe.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://srd.zhengqikj.top

Ruby: Date.parse("2024-01-02")
来源：http://gmg.havefunace.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://aum.yangfankeji.com

[J04] 时间戳与日期互转
来源：http://xep.jiagoushi.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nfb.meibo888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wtq.nanxuanxn.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kvy.gotoacloud.top

TS:   Math.floor(Date.now() / 1000)
来源：http://tvz.bbcook.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rfp.ywan-chungtsiang.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zfy.yonumen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kqu.andypj.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pls.gogol.net.cn

[J05] 时间加减（加 7 天）
来源：http://bpt.yj20258888.top

Py:   now + timedelta(days=7)
来源：http://tpk.hammf.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sei.aizwys.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wrw.shangyingyoupin.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cvr.gzhubu.top

Java: LocalDate.now().plusDays(7)
来源：http://swu.havefunace.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zxy.zhiwuduotai.top

Ruby: Time.now + 7 * 86400
来源：http://ozt.xinyue.icu

C#:   DateTime.Now.AddDays(7)
来源：http://ctf.cqqwz.cn

[J06] 计算两时间之差
来源：http://hsg.yuanzhike.top

Py:   (end - start).total_seconds()
来源：http://cqw.yangfankeji.com

PHP:  $end->diff($start)->days;
来源：http://erc.andypj.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gvs.haohaochexian.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://now.jqgfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://ffh.jinghuilouyu.cn

Go:   end.Sub(start).Hours()
来源：http://fxv.quarkkingdee.top

Ruby: end - start                 # 返回秒数
来源：http://maa.epnwcf.com

C#:   (end - start).TotalSeconds
来源：http://jnf.chenjidiqi.icu

[J07] 比较两个日期
来源：http://pjz.cashguo.top

Py:   d1 < d2;  d1 == d2
来源：http://ked.uphjek.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zqm.cqqwz.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bfh.andypj.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://lzh.shzxlz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gso.daxiang520.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tko.shzxlz.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nvj.pengpengdd.cyou

C#:   d1 < d2;  d1 == d2
来源：http://sco.zdbjq.cn

[J08] 提取年月日与星期
来源：http://rki.gogol.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://itq.havefunace.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kvi.jinqigfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hth.dashuyun.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vxo.hnqzz.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rgq.hnxiangtu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zux.jinyuanbaomall.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qof.jinqigfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gje.jlsjyb.cn

[J09] 时区处理
来源：http://ctl.gogol.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nnu.ivvv.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://isx.guannengcc.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rks.yonumen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yqu.ehwqpu.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kmj.9152youxi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zmn.guowangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xuj.guowangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fue.sweek.top

[J10] 取今天 / 本月第一天
来源：http://jzx.sweek.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rox.tanke756.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://daq.sweek.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dml.haohaochexian.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mwj.zhijiandao.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gxt.guannengcc.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pbh.zhixingplan.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ryg.yj202588.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ljg.ydzc1.top


<!-- 参考信息 -->