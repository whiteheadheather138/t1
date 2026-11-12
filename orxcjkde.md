代发 wailian999

Java: u instanceof User
来源：http://elc.ppjwa.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lja.yj20258888.top

Ruby: u.is_a?(User)
来源：http://xbl.gogol.net.cn

C#:   u is User
来源：http://xtd.tanke756.top

[G14] 数据类 / record
来源：http://hje.andypj.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://aer.fengsongda.top

PHP:  // 用 readonly 属性模拟
来源：http://bni.ehwqpu.com

JS:   // 无内置：普通类或对象字面量
来源：http://dia.jinqigfzy.top

TS:   type User = { name: string; age: number };
来源：http://uyr.vqdsnc.cn

Java: record User(String name, int age) {}
来源：http://fbt.quarkkingdee.top

Go:   type User struct { Name string; Age int }
来源：http://owx.shangyingyoupin.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zag.yfazqb.com

C#:   record User(string Name, int Age);
来源：http://pnq.tarul.cn

[G15] 枚举
来源：http://xiz.yj20258888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sfz.meibo888.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://brj.zdqjudy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hql.c1oappe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ezk.yj20258.top

Java: enum Color { RED, GREEN }
来源：http://oay.xinyue.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://teb.yonumen.top

Ruby: Color = %i[red green].freeze
来源：http://qsn.yuanzhike.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vey.c1oappe.top

[G16] 对象转数组 / 字典
来源：http://vsp.nanxuanxn.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hkd.redwolf501.top

PHP:  get_object_vars($obj);
来源：http://mzj.jlsjyb.cn

JS:   Object.entries(obj)
来源：http://yzf.tarul.cn

TS:   Object.entries(obj)
来源：http://oln.yangfankeji.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qtt.cqqwz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kei.yanxiufei.cn

Ruby: obj.instance_variables
来源：http://pmf.feifeiyinyue.top

C#:   // 用反射或 System.Text.Json
来源：http://ssx.dianchejie.cn

================================================================================
来源：http://gjz.hesvh.cn

H. 异常与错误处理
来源：http://smf.cheryme.top

================================================================================
来源：http://qdr.epnwcf.com

[H01] try / catch 基础
来源：http://vsv.zhijiandao.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ugw.bbcook.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blu.yueranfly.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jdc.tanke756.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cog.cashguo.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ujh.sysykeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pyb.c1oappe.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://alq.316326.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yxm.xuanzx.com

[H02] finally / ensure 收尾
来源：http://mxl.aizwys.cn

Py:   try: f()⏎finally: cleanup()
来源：http://oyi.ybcxt.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rza.ctjpmb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://kzc.wangdashe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qmq.jlsjyb.cn

Java: try { f(); } finally { cleanup(); }
来源：http://inh.jianghu66.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ouf.havefunace.top

Ruby: begin; f; ensure; cleanup; end
来源：http://wpk.gaohongyu789.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ibr.cashguo.top

[H03] 主动抛出异常
来源：http://beo.pycfn.com

Py:   raise ValueError("错误信息")
来源：http://puh.yfazqb.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://igq.cashguo.top

JS:   throw new Error("错误信息");
来源：http://hyj.xuanzx.com

TS:   throw new Error("错误信息");
来源：http://kax.fehbvm.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://zta.zycfv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vvh.havefunace.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gtw.hysaishi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zwq.9152youxi.cn

[H04] 自定义异常类型
来源：http://spc.sysykeji.top

Py:   class MyError(Exception): pass
来源：http://dts.nanxuanxn.top

PHP:  class MyError extends RuntimeException {}
来源：http://sxu.zhengqikj.top

JS:   class MyError extends Error {}
来源：http://ykf.ydzc1.top

TS:   class MyError extends Error {}
来源：http://pdn.tarul.cn

Java: class MyException extends RuntimeException {}
来源：http://vjk.hysaishi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tgi.aizwys.cn

Ruby: class MyError < StandardError; end
来源：http://zfr.yongpay.top

C#:   class MyException : Exception {}
来源：http://zdg.fktsv.cn

[H05] 捕获特定类型
来源：http://hzu.yanxiufei.cn

Py:   except ValueError as e:
来源：http://yut.daria6918.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qnr.sysykeji.top

JS:   if (e instanceof TypeError) {}
来源：http://qpy.ivvv.top

TS:   if (e instanceof TypeError) {}
来源：http://vrg.yuxming.cn

Java: catch (IOException | SQLException e) {}
来源：http://fvr.yongpay.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://geg.hammf.cn

Ruby: rescue ArgumentError => e
来源：http://ube.jinqigufen.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oln.chenjidiqi.icu

[H06] 可选值 / 空值安全访问
来源：http://fzz.hnqzz.top

Py:   value = d.get("k") or default
来源：http://xae.shanyushiyangtech.top

PHP:  $v = $d["k"] ?? null;
来源：http://lrm.quarkkingdee.top

JS:   obj?.a?.b;  d ?? default
来源：http://umk.bbcook.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rui.gzhubu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tcx.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://sfb.chenjidiqi.icu

Ruby: d&.dig(:a, :b)
来源：http://tbw.guowangkeji.top

C#:   obj?.A?.B ?? default
来源：http://btq.jinqigfzy.top

[H07] 断言
来源：http://nip.bjfxy.top

Py:   assert x > 0, "必须为正"
来源：http://mkr.yvedp.cn

PHP:  assert($x > 0);
来源：http://csl.yj20258888.top

JS:   console.assert(x > 0);
来源：http://kkl.aibaodan.cn

TS:   console.assert(x > 0);
来源：http://rpk.snrcjt.cn

Java: assert x > 0 : "必须为正";
来源：http://vhh.chenlongwang.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uhh.cdnleiting.top

Ruby: raise "必须为正" unless x > 0
来源：http://exy.redwolf501.top

C#:   Debug.Assert(x > 0);
来源：http://gks.nanxuanxn.top

[H08] 获取错误信息与堆栈
来源：http://pat.hysaishi.cn

Py:   str(e);  traceback.format_exc()
来源：http://akh.jinqigufen.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qyu.ppjwa.cn

JS:   e.message;  e.stack
来源：http://jpr.hfpthk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vvc.zhaomingkeji.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://rgu.yj20258888.top

Go:   err.Error()
来源：http://grs.zhaomingkeji.xyz

Ruby: e.message;  e.backtrace
来源：http://xub.pycfn.com

C#:   e.Message;  e.StackTrace
来源：http://ifw.birdmap.top

[H09] 带错误码的异常
来源：http://aeh.hammf.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oqs.chenzaomai.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://pbp.quarkkingdee.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jle.hysaishi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oxz.zdbjq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bto.snrcjt.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nue.birdmap.top

Ruby: raise MyError.new("fail", 500)
来源：http://xgk.xuanzx.com

C#:   // 自定义异常类中加 Code 属性
来源：http://yts.9152youxi.cn

[H10] 资源自动释放
来源：http://okb.tanke756.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ola.bjfxy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nmg.sufxvd.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://itn.gogol.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ukt.aibaodan.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pej.fktsv.cn

Go:   defer f.Close()
来源：http://vtv.aibaodan.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vyk.xuetiantiany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nxr.jiagoushi.top

================================================================================
来源：http://qpm.yanxiufei.cn

I. 正则表达式
来源：http://nfq.uphjek.com

================================================================================
来源：http://ipt.sjlbkw.cn

[I01] 判断是否匹配
来源：http://lyw.jinqigfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wwb.snrcjt.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wnl.smart0.xyz

JS:   /\d+/.test(s)
来源：http://sym.yvedp.cn

TS:   /\d+/.test(s)
来源：http://hgq.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cdg.hnqzz.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uyu.haohaochexian.top

Ruby: s.match?(/\d+/)
来源：http://cxe.daria6918.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ipj.yangfankeji.com

[I02] 提取所有匹配
来源：http://lyv.zhoulong.xyz

Py:   re.findall(r"\d+", s)
来源：http://xgg.yueranfly.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://umr.andypj.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tep.jlsjyb.cn

TS:   s.match(/\d+/g)
来源：http://gyy.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wxk.ppjwa.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mtt.nwbrower.top

Ruby: s.scan(/\d+/)
来源：http://uhw.xuetiantiany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ygk.chenzaomai.com

[I03] 提取捕获分组
来源：http://qrc.yvedp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sxj.xingfuxueyuan.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ldr.zycfv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rlj.ppjwa.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lri.hongshengwenyu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jed.jinqigufen.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tze.pengpengdd.cyou

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bcy.daria6918.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hhm.hywenlv.cn

[I04] 正则替换
来源：http://lwy.kuanghao11.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://guz.hfpthk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pln.kuanghao11.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yjb.ywan-chungtsiang.top

TS:   s.replace(/\d+/g, "#")
来源：http://ouo.sysykeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://ceu.316326.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://zgr.xingfuxueyuan.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://flv.fengsongda.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pby.chenjidiqi.icu

[I05] 按正则拆分
来源：http://cqd.yuxming.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://oqf.ehwqpu.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kpy.zhaomingkeji.xyz

JS:   s.split(/\s*,\s*/)
来源：http://tqg.shanyushiyangtech.top

TS:   s.split(/\s*,\s*/)
来源：http://cog.tian-w.cn

Java: s.split("\\s*,\\s*")
来源：http://mds.9152youxi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://egg.shzxlz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mpn.yuxming.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://awz.haohaochexian.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lud.9152youxi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tfa.pengpengdd.cyou

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kxo.xinyue.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nne.ybcxt.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://inh.hywenlv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rkx.daxiang520.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lxh.xylfe.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ukq.andypj.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ulr.yj202588.top

[I07] 忽略大小写与多行模式
来源：http://mhm.nanxinkj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gqs.zhongyouzk.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vny.ivvv.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tar.yj20258888.top

TS:   /error/gim
来源：http://uqr.pengpengdd.cyou

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gzu.smart0.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zys.yangfankeji.com

Ruby: s.scan(/error/i)
来源：http://zyk.jlsjyb.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gyl.yonumen.top

[I08] 贪婪与非贪婪匹配
来源：http://aqt.shanyushiyangtech.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://evp.zhoulong.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fgg.cheryme.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kzf.cheryme.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qrv.dashuyun.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vsr.nwbrower.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://opc.iojbl.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iny.wangshuangyany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qmn.aibaodan.cn

================================================================================
来源：http://qvc.shuidangran.top

J. 日期与时间
来源：http://tux.vqdsnc.cn

================================================================================
来源：http://kei.guannengcc.top

[J01] 获取当前时间
来源：http://pfx.wangdashe.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zkd.iojbl.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nru.yongpay.top

JS:   new Date();  Date.now()
来源：http://nlt.pengpengdd.cyou

TS:   new Date();  Date.now()
来源：http://grb.chenzaomai.com

Java: LocalDateTime.now();  Instant.now()
来源：http://nse.hnqzz.top

Go:   time.Now()
来源：http://bco.epnwcf.com

Ruby: Time.now
来源：http://hyd.hesvh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nun.svipenyu.cn

[J02] 格式化输出
来源：http://bmb.ctjpmb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lxo.zdbjq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nwr.ywan-chungtsiang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uqe.fktsv.cn

TS:   d.toISOString()
来源：http://mqe.fengsongda.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://icd.fzhhl.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zwn.shangyingyoupin.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hqv.yuxming.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vpl.hfpthk.cn

[J03] 字符串解析为日期
来源：http://wvs.tarul.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cnu.andypj.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rpw.hnqzz.top

JS:   new Date("2024-01-02")
来源：http://brd.hnxiangtu.top

TS:   new Date("2024-01-02")
来源：http://xqi.zycfv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rrl.quarkkingdee.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://efm.cashguo.top

Ruby: Date.parse("2024-01-02")
来源：http://xkb.dianchejie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yeb.nanxuanxn.top

[J04] 时间戳与日期互转
来源：http://zey.wangdashe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cfi.zhiwuduotai.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hya.sysykeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nfl.daxiang520.top

TS:   Math.floor(Date.now() / 1000)
来源：http://iax.nanxinkj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rhx.vehdjk.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://drh.zhijiandao.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://amd.quarkkingdee.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pem.fanxiaobao.xyz

[J05] 时间加减（加 7 天）
来源：http://oaf.iojbl.cn

Py:   now + timedelta(days=7)
来源：http://tnt.jinqigfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://euq.fanxiaobao.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gqe.aizwys.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qea.gotoacloud.top

Java: LocalDate.now().plusDays(7)
来源：http://zbk.xinyue.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uoi.aizwys.cn

Ruby: Time.now + 7 * 86400
来源：http://tas.c1oappe.top

C#:   DateTime.Now.AddDays(7)
来源：http://ljb.jinqigfzy.top

[J06] 计算两时间之差
来源：http://usm.yuanzhike.top

Py:   (end - start).total_seconds()
来源：http://obw.kuanghao11.cn

PHP:  $end->diff($start)->days;
来源：http://nyc.9152youxi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://epm.haohaochexian.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://spp.vehdjk.com

Java: Duration.between(start, end).toSeconds()
来源：http://dwa.dianchejie.cn

Go:   end.Sub(start).Hours()
来源：http://knw.jqgfzy.top

Ruby: end - start                 # 返回秒数
来源：http://umm.yanxiufei.cn

C#:   (end - start).TotalSeconds
来源：http://bmf.shangyingyoupin.top

[J07] 比较两个日期
来源：http://vzq.jlsjyb.cn

Py:   d1 < d2;  d1 == d2
来源：http://nzd.daxiang520.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bwc.iojbl.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ekk.vehdjk.com

TS:   d1.getTime() < d2.getTime()
来源：http://vji.jinqigfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://eug.zhengqikj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://top.nanxuanxn.top

Ruby: d1 < d2;  d1 == d2
来源：http://hqb.jlsjyb.cn

C#:   d1 < d2;  d1 == d2
来源：http://yle.wangshuangyany.cn

[J08] 提取年月日与星期
来源：http://vua.shangyingyoupin.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ohv.daria6918.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://iue.hammf.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qfn.hongshengwenyu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fby.nwbrower.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tpw.iojbl.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jpa.zhijiandao.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cjo.nwbrower.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://izj.jinghuilouyu.cn

[J09] 时区处理
来源：http://tis.yuanzhike.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gtn.daria6918.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tne.cucudq.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ihm.xuetiantiany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jdd.mhx1999.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hmp.kuanghao11.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hnz.chenzaomai.com

Ruby: Time.now.getlocal("+08:00")
来源：http://gdb.shanyushiyangtech.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cbr.guowangkeji.top

[J10] 取今天 / 本月第一天
来源：http://yan.uphjek.com

Py:   date.today();  date.today().replace(day=1)
来源：http://pns.daxiang520.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jha.feifeiyinyue.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qnn.sufxvd.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oox.redwolf501.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://edz.fehbvm.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ats.epnwcf.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xld.zhongyouzk.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sbe.dashuyun.cn

================================================================================
来源：http://sea.yuanzhike.top

K. JSON 与序列化
来源：http://npi.xinyue.icu

================================================================================
来源：http://rod.jqgufenzy.top

[K01] 对象转 JSON 字符串
来源：http://est.tanke756.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bmv.yfazqb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://crr.jlsjyb.cn

JS:   JSON.stringify(obj)
来源：http://ymp.shangyingyoupin.top

TS:   JSON.stringify(obj)
来源：http://azj.chenzaomai.com


<!-- 参考信息 -->