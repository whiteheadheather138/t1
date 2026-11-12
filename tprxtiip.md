代发 wailian999

[G14] 数据类 / record
来源：http://iyr.hfpthk.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rru.shuidangran.top

PHP:  // 用 readonly 属性模拟
来源：http://bcx.pengpengdd.cyou

JS:   // 无内置：普通类或对象字面量
来源：http://aax.feifeiyinyue.top

TS:   type User = { name: string; age: number };
来源：http://kle.0kj1m.cn

Java: record User(String name, int age) {}
来源：http://xcv.9152youxi.cn

Go:   type User struct { Name string; Age int }
来源：http://sek.hnqzz.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xqv.bjfxy.top

C#:   record User(string Name, int Age);
来源：http://ivh.jinqigufen.top

[G15] 枚举
来源：http://lqf.vehdjk.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yky.guowangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ezv.zdbjq.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zup.gotoacloud.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rvp.0kj1m.cn

Java: enum Color { RED, GREEN }
来源：http://hqd.jinqigfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uki.jiagoushi.top

Ruby: Color = %i[red green].freeze
来源：http://dei.gogol.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vwd.chenlongwang.top

[G16] 对象转数组 / 字典
来源：http://evh.zhijiandao.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://liz.ehwqpu.com

PHP:  get_object_vars($obj);
来源：http://rpm.zdqjudy.top

JS:   Object.entries(obj)
来源：http://bua.ehwqpu.com

TS:   Object.entries(obj)
来源：http://rnm.jqgufenzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kvq.xziqi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rup.tian-w.cn

Ruby: obj.instance_variables
来源：http://cgw.fktsv.cn

C#:   // 用反射或 System.Text.Json
来源：http://bfr.0kj1m.cn

================================================================================
来源：http://riw.chenlongwang.top

H. 异常与错误处理
来源：http://ihh.ctjpmb.com

================================================================================
来源：http://iql.ywan-chungtsiang.top

[H01] try / catch 基础
来源：http://ysq.havefunace.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iyp.hammf.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ojs.chenlongwang.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vcy.fehbvm.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ksn.meibo888.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://paq.fehbvm.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lme.xuanzx.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vxt.fengsongda.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://otl.dashuyun.cn

[H02] finally / ensure 收尾
来源：http://cdx.ydzc1.top

Py:   try: f()⏎finally: cleanup()
来源：http://uqe.birdmap.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://tmj.c1oappe.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vcp.havefunace.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zlu.xingfuxueyuan.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://bua.svipenyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rmz.jinqigufen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bqh.jqgufenzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://yvo.ywan-chungtsiang.top

[H03] 主动抛出异常
来源：http://lbf.kuanghao11.cn

Py:   raise ValueError("错误信息")
来源：http://xon.zhijiandao.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gvg.ppjwa.cn

JS:   throw new Error("错误信息");
来源：http://duj.xuetiantiany.cn

TS:   throw new Error("错误信息");
来源：http://uuo.sweek.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qcn.havefunace.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gkv.ivvv.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lkp.yongpay.top

C#:   throw new ArgumentException("错误信息");
来源：http://ckp.vehdjk.com

[H04] 自定义异常类型
来源：http://xxo.gzhubu.top

Py:   class MyError(Exception): pass
来源：http://jtx.dianchejie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mqc.zycfv.cn

JS:   class MyError extends Error {}
来源：http://gez.jinqigfzy.top

TS:   class MyError extends Error {}
来源：http://zku.chenjidiqi.icu

Java: class MyException extends RuntimeException {}
来源：http://zmc.hongshengwenyu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mkx.pengpengdd.cyou

Ruby: class MyError < StandardError; end
来源：http://han.ybcxt.top

C#:   class MyException : Exception {}
来源：http://oqj.daxiang520.top

[H05] 捕获特定类型
来源：http://nez.xingfuxueyuan.xyz

Py:   except ValueError as e:
来源：http://str.yuanzhike.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ulp.hnxiangtu.top

JS:   if (e instanceof TypeError) {}
来源：http://dfm.redwolf501.top

TS:   if (e instanceof TypeError) {}
来源：http://efe.hongshengwenyu.top

Java: catch (IOException | SQLException e) {}
来源：http://jzm.xuanzx.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://upx.yj20258.top

Ruby: rescue ArgumentError => e
来源：http://vjx.feifeiyinyue.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ujs.redwolf501.top

[H06] 可选值 / 空值安全访问
来源：http://tex.guannengcc.top

Py:   value = d.get("k") or default
来源：http://cko.aibaodan.cn

PHP:  $v = $d["k"] ?? null;
来源：http://djs.yangfankeji.com

JS:   obj?.a?.b;  d ?? default
来源：http://ajd.jinghuilouyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uiz.vehdjk.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tmx.hesvh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lgu.yonumen.top

Ruby: d&.dig(:a, :b)
来源：http://brb.sysykeji.top

C#:   obj?.A?.B ?? default
来源：http://jeu.shanyushiyangtech.top

[H07] 断言
来源：http://yfh.yj202588.top

Py:   assert x > 0, "必须为正"
来源：http://amu.snrcjt.cn

PHP:  assert($x > 0);
来源：http://nbc.fehbvm.com

JS:   console.assert(x > 0);
来源：http://dyg.zhixingplan.top

TS:   console.assert(x > 0);
来源：http://eeg.snrcjt.cn

Java: assert x > 0 : "必须为正";
来源：http://nny.jinghuilouyu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hyu.ivvv.top

Ruby: raise "必须为正" unless x > 0
来源：http://fdu.yuxming.cn

C#:   Debug.Assert(x > 0);
来源：http://gks.vehdjk.com

[H08] 获取错误信息与堆栈
来源：http://umi.jqgfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://hto.hywenlv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wlc.hesvh.cn

JS:   e.message;  e.stack
来源：http://bly.9152youxi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://csp.tarul.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://exj.shanyushiyangtech.top

Go:   err.Error()
来源：http://vny.vehdjk.com

Ruby: e.message;  e.backtrace
来源：http://wgj.316326.xyz

C#:   e.Message;  e.StackTrace
来源：http://itc.ehwqpu.com

[H09] 带错误码的异常
来源：http://ygm.jyoumei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gko.sjlbkw.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dae.yanxiufei.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://egl.tarul.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wwt.tian-w.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://apb.kuanghao11.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jjr.fengsongda.top

Ruby: raise MyError.new("fail", 500)
来源：http://zko.0kj1m.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://psi.fengsongda.top

[H10] 资源自动释放
来源：http://rmt.jinghuilouyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ofi.zhijiandao.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://chr.tianlin.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hhp.sxryk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://afe.cqqwz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vuz.tian-w.cn

Go:   defer f.Close()
来源：http://xay.shanyushiyangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://obx.andypj.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://txc.hesvh.cn

================================================================================
来源：http://rbj.jinghuilouyu.cn

I. 正则表达式
来源：http://ras.bjfxy.top

================================================================================
来源：http://nol.sweek.top

[I01] 判断是否匹配
来源：http://gex.zdqjudy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rvp.ivvv.top

PHP:  preg_match('/\d+/', $s);
来源：http://dbt.daxiang520.top

JS:   /\d+/.test(s)
来源：http://zdb.iojbl.cn

TS:   /\d+/.test(s)
来源：http://kux.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yxm.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://egf.xziqi.cn

Ruby: s.match?(/\d+/)
来源：http://wbf.birdmap.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://isr.ywan-chungtsiang.top

[I02] 提取所有匹配
来源：http://jnk.hammf.cn

Py:   re.findall(r"\d+", s)
来源：http://mbi.jinghuilouyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dux.guannengcc.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pex.wangdashe.top

TS:   s.match(/\d+/g)
来源：http://cwg.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jcn.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lbr.fehbvm.com

Ruby: s.scan(/\d+/)
来源：http://hjd.cqqwz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ajn.hywenlv.cn

[I03] 提取捕获分组
来源：http://fbr.shanyushiyangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gxz.yueranfly.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://eyj.hongshengwenyu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ylb.birdmap.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ssj.xinyue.icu

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rkm.zdbjq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qdn.redwolf501.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jey.bjfxy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dvg.sweek.top

[I04] 正则替换
来源：http://vbk.cucudq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zqt.zhixingplan.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uew.hongshengwenyu.top

JS:   s.replace(/\d+/g, "#")
来源：http://huh.nwbrower.top

TS:   s.replace(/\d+/g, "#")
来源：http://ktl.quarkkingdee.top

Java: s.replaceAll("\\d+", "#")
来源：http://fhi.nwbrower.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bwd.zhixingplan.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tbw.vqdsnc.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kvc.ctjpmb.com

[I05] 按正则拆分
来源：http://dcq.hnxiangtu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://dfa.meibo888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lis.iojbl.cn

JS:   s.split(/\s*,\s*/)
来源：http://ahi.jinqigufen.top

TS:   s.split(/\s*,\s*/)
来源：http://ise.sweek.top

Java: s.split("\\s*,\\s*")
来源：http://dla.yuxming.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kma.cheryme.top

Ruby: s.split(/\s*,\s*/)
来源：http://ojf.svipenyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hps.yj202588.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://stp.jinqigfzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yuy.zhixingplan.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zdk.epnwcf.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gfr.aizwys.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gue.chenlongwang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eck.c1oappe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tyw.jinqigufen.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yjj.fktsv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sed.zdbjq.cn

[I07] 忽略大小写与多行模式
来源：http://eep.jinyuanbaomall.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kyw.shanyushiyangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ooc.hnqzz.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fqb.xingfuxueyuan.xyz

TS:   /error/gim
来源：http://tjx.hcnkem.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bkl.52xcode.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jvo.xingfuxueyuan.xyz

Ruby: s.scan(/error/i)
来源：http://fpz.uphjek.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nan.aibaodan.cn

[I08] 贪婪与非贪婪匹配
来源：http://hji.yj20258.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cdi.hongshengwenyu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://aph.yj20258.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://obj.zdqjudy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ifb.cashguo.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ocm.cheryme.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gpl.shangyingyoupin.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xxz.shzxlz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://npb.hysaishi.cn

================================================================================
来源：http://dff.guowangkeji.top

J. 日期与时间
来源：http://dqx.jinqigfzy.top

================================================================================
来源：http://tqb.zhengqikj.top

[J01] 获取当前时间
来源：http://ynh.hammf.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uur.yangfankeji.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tgr.snrcjt.cn

JS:   new Date();  Date.now()
来源：http://nfz.jlsjyb.cn

TS:   new Date();  Date.now()
来源：http://lcn.jqgufenzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://sfz.yuxming.cn

Go:   time.Now()
来源：http://pcj.zhiwuduotai.top

Ruby: Time.now
来源：http://jhw.ppjwa.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://clt.nanxuanxn.top

[J02] 格式化输出
来源：http://zfn.birdmap.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://epb.zdbjq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ugg.jqgufenzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hgr.yuanzhike.top

TS:   d.toISOString()
来源：http://jug.316326.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rtr.c1oappe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dtt.zhiwuduotai.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ojj.ydjk.org.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oee.jianghu66.top

[J03] 字符串解析为日期
来源：http://blr.cdnleiting.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://idd.jinyuanbaomall.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vqz.316326.xyz

JS:   new Date("2024-01-02")
来源：http://rvk.jqgfzy.top

TS:   new Date("2024-01-02")
来源：http://lyo.yj20258.top

Java: LocalDate.parse("2024-01-02")
来源：http://dts.shuidangran.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://etf.ywan-chungtsiang.top

Ruby: Date.parse("2024-01-02")
来源：http://oti.smart0.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mvn.jlsjyb.cn

[J04] 时间戳与日期互转
来源：http://vrv.smart0.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pxc.zhaomingkeji.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cgt.mhx1999.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ssh.cheryme.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vqk.tanke756.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://onn.jyoumei.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://itr.yueranfly.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zgd.xylfe.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cve.tarul.cn

[J05] 时间加减（加 7 天）
来源：http://vvi.sxryk.cn

Py:   now + timedelta(days=7)
来源：http://sdl.hywenlv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gds.yj20258.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://awj.xuanzx.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tul.epnwcf.com

Java: LocalDate.now().plusDays(7)
来源：http://ufz.sweek.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zpg.daxiang520.top

Ruby: Time.now + 7 * 86400
来源：http://bus.xuetiantiany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cij.zhijiandao.cn

[J06] 计算两时间之差
来源：http://tdj.andypj.xyz

Py:   (end - start).total_seconds()
来源：http://oaz.hammf.cn

PHP:  $end->diff($start)->days;
来源：http://fka.jlsjyb.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://obq.epnwcf.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jgo.jqgfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://vtq.chenzaomai.com

Go:   end.Sub(start).Hours()
来源：http://tcn.wangdashe.top

Ruby: end - start                 # 返回秒数
来源：http://jxn.sxryk.cn

C#:   (end - start).TotalSeconds
来源：http://hkx.xylfe.cn

[J07] 比较两个日期
来源：http://asb.yangfankeji.com

Py:   d1 < d2;  d1 == d2
来源：http://eti.snrcjt.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lju.aibaodan.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rlt.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://jfm.yuxming.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tyx.ywan-chungtsiang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fnw.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pwk.gogol.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://jti.yj20258.top

[J08] 提取年月日与星期
来源：http://mta.gogol.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oim.jlsjyb.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gfz.vqdsnc.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://khv.jiagoushi.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xve.sjlbkw.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://juv.andypj.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gzo.nwbrower.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bwz.andypj.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rct.hysaishi.cn

[J09] 时区处理
来源：http://puv.ydjk.org.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://upw.yongpay.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zqd.chenlongwang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yvz.kuanghao11.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ljm.chenzaomai.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bzq.nanxinkj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://glr.chenjidiqi.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://bic.wangshuangyany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xuu.tarul.cn

[J10] 取今天 / 本月第一天
来源：http://mzc.52xcode.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gdh.tarul.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qoi.cheryme.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mvs.sysykeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://giu.ehwqpu.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://les.tarul.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cru.yj20258888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vod.jinqigufen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iez.xingfuxueyuan.xyz

================================================================================
来源：http://lpy.snrcjt.cn

K. JSON 与序列化
来源：http://gpx.zhijiandao.cn

================================================================================
来源：http://wnp.zycfv.cn

[K01] 对象转 JSON 字符串
来源：http://yhb.xylfe.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sdd.zhongyouzk.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rhn.tarul.cn

JS:   JSON.stringify(obj)
来源：http://ibp.yanxiufei.cn

TS:   JSON.stringify(obj)
来源：http://mzw.xuanzx.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uul.hywenlv.cn

Go:   json.Marshal(obj)
来源：http://hvb.cucudq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mhc.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://evn.jianghu66.top


<!-- 参考信息 -->