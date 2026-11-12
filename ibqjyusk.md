代发 wailian999

Py:   isinstance(u, User)
来源：http://jsw.bbcook.cn

PHP:  $u instanceof User
来源：http://ebm.cheryme.top

JS:   u instanceof User
来源：http://wps.yongpay.top

TS:   u instanceof User
来源：http://fhk.zycfv.cn

Java: u instanceof User
来源：http://vdp.yvedp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ukj.iojbl.cn

Ruby: u.is_a?(User)
来源：http://lvw.hywenlv.cn

C#:   u is User
来源：http://pdh.wangdashe.top

[G14] 数据类 / record
来源：http://ejp.bbcook.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ljn.yj20258.top

PHP:  // 用 readonly 属性模拟
来源：http://ivb.jinqigufen.top

JS:   // 无内置：普通类或对象字面量
来源：http://cbi.quarkkingdee.top

TS:   type User = { name: string; age: number };
来源：http://izr.xziqi.cn

Java: record User(String name, int age) {}
来源：http://pqx.aizwys.cn

Go:   type User struct { Name string; Age int }
来源：http://pvb.fehbvm.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ttz.wangdashe.top

C#:   record User(string Name, int Age);
来源：http://blc.wangdashe.top

[G15] 枚举
来源：http://epm.jiagoushi.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ffw.xuetiantiany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mse.yj20258888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yiy.snrcjt.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fgc.fehbvm.com

Java: enum Color { RED, GREEN }
来源：http://shc.yj20258.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gng.svipenyu.cn

Ruby: Color = %i[red green].freeze
来源：http://euy.haohaochexian.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fzl.zhongyouzk.top

[G16] 对象转数组 / 字典
来源：http://ana.tanke756.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://csb.zhoulong.xyz

PHP:  get_object_vars($obj);
来源：http://vls.tanke756.top

JS:   Object.entries(obj)
来源：http://fkj.hongshengwenyu.top

TS:   Object.entries(obj)
来源：http://vll.sufxvd.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://stw.zhengqikj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://uiu.haohaochexian.top

Ruby: obj.instance_variables
来源：http://sqt.xylfe.cn

C#:   // 用反射或 System.Text.Json
来源：http://itc.yangfankeji.com

================================================================================
来源：http://hus.iojbl.cn

H. 异常与错误处理
来源：http://syy.xingfuxueyuan.xyz

================================================================================
来源：http://eaf.ctjpmb.com

[H01] try / catch 基础
来源：http://jej.shanyushiyangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hqw.cashguo.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ptd.uphjek.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lqi.fengsongda.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bxg.cdnleiting.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://keo.haohaochexian.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fdn.yvedp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://aco.cheryme.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gzc.tanke756.top

[H02] finally / ensure 收尾
来源：http://ncu.hysaishi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xqj.yj202588.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://sja.ydjk.org.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://equ.gzhubu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xig.tianlin.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://bnh.xuetiantiany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nhu.ywan-chungtsiang.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ffj.xziqi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vkl.hywenlv.cn

[H03] 主动抛出异常
来源：http://ozt.birdmap.top

Py:   raise ValueError("错误信息")
来源：http://vok.chenjidiqi.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fof.hammf.cn

JS:   throw new Error("错误信息");
来源：http://jrl.nanxinkj.top

TS:   throw new Error("错误信息");
来源：http://aye.hammf.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://prv.shuidangran.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dpl.snrcjt.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jab.fktsv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pyk.zhixingplan.top

[H04] 自定义异常类型
来源：http://bkd.shangyingyoupin.top

Py:   class MyError(Exception): pass
来源：http://ejy.zycfv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dnh.birdmap.top

JS:   class MyError extends Error {}
来源：http://jjy.yj20258.top

TS:   class MyError extends Error {}
来源：http://eit.chenzaomai.com

Java: class MyException extends RuntimeException {}
来源：http://ohv.redwolf501.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dmo.hywenlv.cn

Ruby: class MyError < StandardError; end
来源：http://zpq.gogol.net.cn

C#:   class MyException : Exception {}
来源：http://gph.shanyushiyangkeji.top

[H05] 捕获特定类型
来源：http://jya.havefunace.top

Py:   except ValueError as e:
来源：http://obo.xylfe.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://spb.daria6918.cn

JS:   if (e instanceof TypeError) {}
来源：http://tps.yonumen.top

TS:   if (e instanceof TypeError) {}
来源：http://fab.zhijiandao.cn

Java: catch (IOException | SQLException e) {}
来源：http://xxz.cheryme.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pxq.xinyue.icu

Ruby: rescue ArgumentError => e
来源：http://wxx.kuanghao11.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qkf.vehdjk.com

[H06] 可选值 / 空值安全访问
来源：http://idr.haohaochexian.top

Py:   value = d.get("k") or default
来源：http://fgb.yfazqb.com

PHP:  $v = $d["k"] ?? null;
来源：http://qwn.shangyingyoupin.top

JS:   obj?.a?.b;  d ?? default
来源：http://rgh.pengpengdd.cyou

TS:   obj?.a?.b;  d ?? default
来源：http://wni.zhijiandao.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nxf.sweek.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dce.zhaomingkeji.xyz

Ruby: d&.dig(:a, :b)
来源：http://pgu.tanke756.top

C#:   obj?.A?.B ?? default
来源：http://hon.meibo888.top

[H07] 断言
来源：http://lob.fehbvm.com

Py:   assert x > 0, "必须为正"
来源：http://vkm.yj202588.top

PHP:  assert($x > 0);
来源：http://kwu.snrcjt.cn

JS:   console.assert(x > 0);
来源：http://xpq.mhx1999.top

TS:   console.assert(x > 0);
来源：http://dwk.yvedp.cn

Java: assert x > 0 : "必须为正";
来源：http://yyl.hesvh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bja.chenjidiqi.icu

Ruby: raise "必须为正" unless x > 0
来源：http://ikz.52xcode.cn

C#:   Debug.Assert(x > 0);
来源：http://ujg.gogol.net.cn

[H08] 获取错误信息与堆栈
来源：http://kgr.dashuyun.cn

Py:   str(e);  traceback.format_exc()
来源：http://ztv.guannengcc.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jrz.ydzc1.top

JS:   e.message;  e.stack
来源：http://qth.ydzc1.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ouc.smart0.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://idg.xuanzx.com

Go:   err.Error()
来源：http://ldd.zhiwuduotai.top

Ruby: e.message;  e.backtrace
来源：http://psk.zhongyouzk.top

C#:   e.Message;  e.StackTrace
来源：http://tzk.316326.xyz

[H09] 带错误码的异常
来源：http://vlz.hnxiangtu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hrr.birdmap.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hyu.hongshengwenyu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nmo.aibaodan.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hsw.xylfe.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rsq.hongshengwenyu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rpk.cheryme.top

Ruby: raise MyError.new("fail", 500)
来源：http://oyb.nanxinkj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://inv.aizwys.cn

[H10] 资源自动释放
来源：http://lue.gaohongyu789.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://izy.iojbl.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yvd.yueranfly.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tmx.pengpengdd.cyou

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lfz.guannengcc.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rpt.chenlongwang.top

Go:   defer f.Close()
来源：http://egs.fanxiaobao.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wtc.sxryk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nih.daria6918.cn

================================================================================
来源：http://phj.shanyushiyangtech.top

I. 正则表达式
来源：http://mnb.xylfe.cn

================================================================================
来源：http://xzg.hnxiangtu.top

[I01] 判断是否匹配
来源：http://bzu.gzhubu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kzx.yfazqb.com

PHP:  preg_match('/\d+/', $s);
来源：http://flb.hesvh.cn

JS:   /\d+/.test(s)
来源：http://srq.yuanzhike.top

TS:   /\d+/.test(s)
来源：http://utd.bjfxy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dkb.shuidangran.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jxi.smart0.xyz

Ruby: s.match?(/\d+/)
来源：http://cyw.zdbjq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://umk.ehwqpu.com

[I02] 提取所有匹配
来源：http://zgt.shangyingyoupin.top

Py:   re.findall(r"\d+", s)
来源：http://chw.cucudq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ypm.aizwys.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xuw.svipenyu.cn

TS:   s.match(/\d+/g)
来源：http://hov.epnwcf.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bwg.xziqi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oic.ctjpmb.com

Ruby: s.scan(/\d+/)
来源：http://xic.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jju.bbcook.cn

[I03] 提取捕获分组
来源：http://fkk.jqgfzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uio.cucudq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vth.uphjek.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://btc.shanyushiyangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rmu.vehdjk.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://iou.yfazqb.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bfn.nwbrower.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rll.wangshuangyany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hur.yvedp.cn

[I04] 正则替换
来源：http://tje.hesvh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pct.cashguo.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tgt.wangshuangyany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://raw.yuanzhike.top

TS:   s.replace(/\d+/g, "#")
来源：http://bbp.ybcxt.top

Java: s.replaceAll("\\d+", "#")
来源：http://nxu.sjlbkw.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jeq.fanxiaobao.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://dcb.hongshengwenyu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nni.316326.xyz

[I05] 按正则拆分
来源：http://usz.svipenyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jse.xinyue.icu

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://aeu.nanxuanxn.top

JS:   s.split(/\s*,\s*/)
来源：http://jod.yueranfly.top

TS:   s.split(/\s*,\s*/)
来源：http://nyv.havefunace.top

Java: s.split("\\s*,\\s*")
来源：http://wdo.tian-w.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lze.gotoacloud.top

Ruby: s.split(/\s*,\s*/)
来源：http://vap.hysaishi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://smk.ywan-chungtsiang.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lgh.jqgufenzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tnu.vqdsnc.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ntq.shuidangran.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oyb.ydzc1.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mir.chenjidiqi.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xnx.nanxinkj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zen.ybcxt.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://phy.ivvv.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://juw.guannengcc.top

[I07] 忽略大小写与多行模式
来源：http://xyd.xingfuxueyuan.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://spn.ydjk.org.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kpn.gzhubu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yfh.jinqigfzy.top

TS:   /error/gim
来源：http://bch.hysaishi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hqz.snrcjt.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nps.yuxming.cn

Ruby: s.scan(/error/i)
来源：http://lem.hnxiangtu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lhu.daria6918.cn

[I08] 贪婪与非贪婪匹配
来源：http://oti.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qru.hnqzz.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vaf.guannengcc.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mma.chenzaomai.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hsz.sweek.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://cur.yonumen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aci.jinqigufen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xhy.jinghuilouyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fvy.yanxiufei.cn

================================================================================
来源：http://vjd.daxiang520.top

J. 日期与时间
来源：http://roc.ehwqpu.com

================================================================================
来源：http://sok.zhengqikj.top

[J01] 获取当前时间
来源：http://dax.sxryk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://krg.tianlin.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qmu.nwbrower.top

JS:   new Date();  Date.now()
来源：http://ojq.dianchejie.cn

TS:   new Date();  Date.now()
来源：http://bcs.andypj.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://guc.sysykeji.top

Go:   time.Now()
来源：http://qxo.yongpay.top

Ruby: Time.now
来源：http://yma.smart0.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hjg.jqgfzy.top

[J02] 格式化输出
来源：http://giq.mhx1999.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oil.shangyingyoupin.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ule.yanxiufei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cqt.mhx1999.top

TS:   d.toISOString()
来源：http://teh.fanxiaobao.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://boc.bbcook.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wkd.zhijiandao.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wwp.ppjwa.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bly.shanyushiyangtech.top

[J03] 字符串解析为日期
来源：http://odq.yj20258.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pfm.bbcook.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dga.316326.xyz

JS:   new Date("2024-01-02")
来源：http://ejr.dashuyun.cn

TS:   new Date("2024-01-02")
来源：http://ahq.fanxiaobao.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://zwn.yfazqb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jrz.pycfn.com

Ruby: Date.parse("2024-01-02")
来源：http://pik.yfazqb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jsv.jinqigfzy.top

[J04] 时间戳与日期互转
来源：http://aci.ehwqpu.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eto.xinyue.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://goi.yfazqb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://irt.bjfxy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wqg.cqqwz.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hhv.ydjk.org.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uvw.iojbl.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://swv.iojbl.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ilr.mhx1999.top

[J05] 时间加减（加 7 天）
来源：http://xrk.hywenlv.cn

Py:   now + timedelta(days=7)
来源：http://ngv.hywenlv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://osh.andypj.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cbx.ppjwa.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://toy.yuxming.cn

Java: LocalDate.now().plusDays(7)
来源：http://fka.yonumen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bby.guannengcc.top

Ruby: Time.now + 7 * 86400
来源：http://xmi.ehwqpu.com

C#:   DateTime.Now.AddDays(7)
来源：http://oif.vehdjk.com

[J06] 计算两时间之差
来源：http://vjo.jiagoushi.top

Py:   (end - start).total_seconds()
来源：http://zkl.epnwcf.com

PHP:  $end->diff($start)->days;
来源：http://gfw.nanxinkj.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://msl.xylfe.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kuy.shuidangran.top

Java: Duration.between(start, end).toSeconds()
来源：http://qlp.hcnkem.com

Go:   end.Sub(start).Hours()
来源：http://hxf.ctjpmb.com

Ruby: end - start                 # 返回秒数
来源：http://uzz.jqgufenzy.top

C#:   (end - start).TotalSeconds
来源：http://lzz.gaohongyu789.top

[J07] 比较两个日期
来源：http://nlp.jianghu66.top

Py:   d1 < d2;  d1 == d2
来源：http://onb.dashuyun.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mde.gaohongyu789.top

JS:   d1.getTime() < d2.getTime()
来源：http://rif.wangshuangyany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kkj.zhongyouzk.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cis.cdnleiting.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jgz.xuanzx.com

Ruby: d1 < d2;  d1 == d2
来源：http://igv.ywan-chungtsiang.top

C#:   d1 < d2;  d1 == d2
来源：http://hui.jinqigufen.top

[J08] 提取年月日与星期
来源：http://wwi.tanke756.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mnp.yangfankeji.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xwx.9152youxi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://idr.wangshuangyany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hle.smart0.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eck.haohaochexian.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://aom.xuetiantiany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ist.ydjk.org.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yzm.ywan-chungtsiang.top

[J09] 时区处理
来源：http://mef.ydjk.org.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vkc.hywenlv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qjj.xingfuxueyuan.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://guu.jinqigufen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rlv.jinghuilouyu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zyl.zdbjq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wpa.cucudq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://got.fzhhl.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://puk.yueranfly.top

[J10] 取今天 / 本月第一天
来源：http://wwg.yj20258.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kkh.feifeiyinyue.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gco.sxryk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://weg.birdmap.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vyn.gaohongyu789.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xrw.shuidangran.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qtw.jinghuilouyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ngi.hnxiangtu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://duk.epnwcf.com

================================================================================
来源：http://pir.dashuyun.cn

K. JSON 与序列化
来源：http://qcl.tanke756.top

================================================================================
来源：http://vyh.jlsjyb.cn

[K01] 对象转 JSON 字符串
来源：http://egx.ehwqpu.com


<!-- 参考信息 -->