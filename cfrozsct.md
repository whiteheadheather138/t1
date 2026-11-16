代发 wailian999

Java: u instanceof User
来源：http://bji.ppjwa.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hnf.sufxvd.cn

Ruby: u.is_a?(User)
来源：http://kqw.fktsv.cn

C#:   u is User
来源：http://bru.ybcxt.top

[G14] 数据类 / record
来源：http://zzq.vehdjk.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hpp.daria6918.cn

PHP:  // 用 readonly 属性模拟
来源：http://fgd.yj20258.top

JS:   // 无内置：普通类或对象字面量
来源：http://xoi.cdnleiting.top

TS:   type User = { name: string; age: number };
来源：http://hzj.jiagoushi.top

Java: record User(String name, int age) {}
来源：http://wyn.yuxming.cn

Go:   type User struct { Name string; Age int }
来源：http://wjb.meibo888.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jiz.yj202588.top

C#:   record User(string Name, int Age);
来源：http://dbs.sjlbkw.cn

[G15] 枚举
来源：http://dvo.guannengcc.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uvh.aibaodan.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gxz.tianlin.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ebb.bbcook.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jaw.nwbrower.top

Java: enum Color { RED, GREEN }
来源：http://gnq.yj20258888.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://djn.fehbvm.com

Ruby: Color = %i[red green].freeze
来源：http://bgs.jinqigfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iml.havefunace.top

[G16] 对象转数组 / 字典
来源：http://elu.pycfn.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xht.yj20258888.top

PHP:  get_object_vars($obj);
来源：http://joh.hnqzz.top

JS:   Object.entries(obj)
来源：http://iht.shuidangran.top

TS:   Object.entries(obj)
来源：http://pwb.xziqi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fhc.hfpthk.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bpo.xuanzx.com

Ruby: obj.instance_variables
来源：http://gih.hnxiangtu.top

C#:   // 用反射或 System.Text.Json
来源：http://vrr.shuidangran.top

================================================================================
来源：http://mcz.wangdashe.top

H. 异常与错误处理
来源：http://goy.chenzaomai.com

================================================================================
来源：http://bwu.sweek.top

[H01] try / catch 基础
来源：http://ivh.yfazqb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uss.guannengcc.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gft.ivvv.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tve.cdnleiting.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qjf.chenlongwang.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ecr.hongshengwenyu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vln.yuxming.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rpe.xingfuxueyuan.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mmn.iojbl.cn

[H02] finally / ensure 收尾
来源：http://dve.xinyue.icu

Py:   try: f()⏎finally: cleanup()
来源：http://aln.jinqigfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://wzv.jlsjyb.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jtq.wangshuangyany.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sdj.aibaodan.cn

Java: try { f(); } finally { cleanup(); }
来源：http://utm.jinghuilouyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wpf.cucudq.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dad.mhx1999.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ity.daxiang520.top

[H03] 主动抛出异常
来源：http://ply.hongshengwenyu.top

Py:   raise ValueError("错误信息")
来源：http://qiq.xziqi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ker.dianchejie.cn

JS:   throw new Error("错误信息");
来源：http://kvk.ybcxt.top

TS:   throw new Error("错误信息");
来源：http://otm.yvedp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cbc.jinghuilouyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rdt.xziqi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vcr.xziqi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pvs.snrcjt.cn

[H04] 自定义异常类型
来源：http://mmw.chenlongwang.top

Py:   class MyError(Exception): pass
来源：http://dot.zhoulong.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://ukm.zycfv.cn

JS:   class MyError extends Error {}
来源：http://pbb.xylfe.cn

TS:   class MyError extends Error {}
来源：http://ukg.tarul.cn

Java: class MyException extends RuntimeException {}
来源：http://sle.sysykeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bsd.zhijiandao.cn

Ruby: class MyError < StandardError; end
来源：http://ixy.fengsongda.top

C#:   class MyException : Exception {}
来源：http://wif.zdbjq.cn

[H05] 捕获特定类型
来源：http://shy.yvedp.cn

Py:   except ValueError as e:
来源：http://elf.shzxlz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sdc.jqgfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://bgz.yuanzhike.top

TS:   if (e instanceof TypeError) {}
来源：http://trk.jinqigufen.top

Java: catch (IOException | SQLException e) {}
来源：http://ucj.52xcode.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ohj.shanyushiyangkeji.top

Ruby: rescue ArgumentError => e
来源：http://evo.hesvh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rrv.zdbjq.cn

[H06] 可选值 / 空值安全访问
来源：http://bbq.ctjpmb.com

Py:   value = d.get("k") or default
来源：http://psn.shanyushiyangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://wut.ybcxt.top

JS:   obj?.a?.b;  d ?? default
来源：http://bje.aibaodan.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mht.ydzc1.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yrb.shanyushiyangkeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ici.epnwcf.com

Ruby: d&.dig(:a, :b)
来源：http://cag.sysykeji.top

C#:   obj?.A?.B ?? default
来源：http://vnw.ppjwa.cn

[H07] 断言
来源：http://zar.jqgfzy.top

Py:   assert x > 0, "必须为正"
来源：http://thk.snrcjt.cn

PHP:  assert($x > 0);
来源：http://mnv.jyoumei.cn

JS:   console.assert(x > 0);
来源：http://jrh.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://dkz.yuanzhike.top

Java: assert x > 0 : "必须为正";
来源：http://mxz.cheryme.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://egt.zhengqikj.top

Ruby: raise "必须为正" unless x > 0
来源：http://tfi.hysaishi.cn

C#:   Debug.Assert(x > 0);
来源：http://jpm.zhixingplan.top

[H08] 获取错误信息与堆栈
来源：http://uxp.zhoulong.xyz

Py:   str(e);  traceback.format_exc()
来源：http://gtu.hywenlv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jem.nanxuanxn.top

JS:   e.message;  e.stack
来源：http://aaq.jqgufenzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://nbq.cqqwz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://oha.jinqigfzy.top

Go:   err.Error()
来源：http://kfx.fktsv.cn

Ruby: e.message;  e.backtrace
来源：http://mhs.hcnkem.com

C#:   e.Message;  e.StackTrace
来源：http://cek.hammf.cn

[H09] 带错误码的异常
来源：http://wab.chenlongwang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://aew.sysykeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hys.hesvh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ejj.9152youxi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wof.hfpthk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wjl.nanxinkj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iii.iojbl.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ygb.xingfuxueyuan.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://fix.zhixingplan.top

[H10] 资源自动释放
来源：http://ktl.hnqzz.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kgk.birdmap.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mfb.ybcxt.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pbi.gaohongyu789.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yoi.cqqwz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yvh.iojbl.cn

Go:   defer f.Close()
来源：http://htw.fktsv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bjf.fehbvm.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xmq.fanxiaobao.xyz

================================================================================
来源：http://shw.guannengcc.top

I. 正则表达式
来源：http://rmd.quarkkingdee.top

================================================================================
来源：http://lin.cqqwz.cn

[I01] 判断是否匹配
来源：http://ueu.zhoulong.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://das.birdmap.top

PHP:  preg_match('/\d+/', $s);
来源：http://zsd.zycfv.cn

JS:   /\d+/.test(s)
来源：http://bsy.ydjk.org.cn

TS:   /\d+/.test(s)
来源：http://efq.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://esv.sxryk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ywm.quarkkingdee.top

Ruby: s.match?(/\d+/)
来源：http://hnn.ehwqpu.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xfa.zdqjudy.top

[I02] 提取所有匹配
来源：http://own.jyoumei.cn

Py:   re.findall(r"\d+", s)
来源：http://xww.shangyingyoupin.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://exy.ivvv.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jwz.ivvv.top

TS:   s.match(/\d+/g)
来源：http://idv.tianlin.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jlz.bjfxy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://trh.jqgufenzy.top

Ruby: s.scan(/\d+/)
来源：http://ypm.daxiang520.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wvf.quarkkingdee.top

[I03] 提取捕获分组
来源：http://vhw.nanxuanxn.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dat.jinyuanbaomall.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pga.haohaochexian.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lky.wangdashe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fbo.zhixingplan.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kek.ybcxt.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tam.iojbl.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tta.jiagoushi.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iyu.ybcxt.top

[I04] 正则替换
来源：http://yxc.ivvv.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fef.sweek.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oic.tarul.cn

JS:   s.replace(/\d+/g, "#")
来源：http://onu.wangdashe.top

TS:   s.replace(/\d+/g, "#")
来源：http://rka.jinghuilouyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qic.zhijiandao.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ewc.jqgfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kfk.yj20258.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nhv.cashguo.top

[I05] 按正则拆分
来源：http://mhu.pycfn.com

Py:   re.split(r"\s*,\s*", s)
来源：http://erm.vehdjk.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lor.ydzc1.top

JS:   s.split(/\s*,\s*/)
来源：http://vgr.uphjek.com

TS:   s.split(/\s*,\s*/)
来源：http://xhf.haohaochexian.top

Java: s.split("\\s*,\\s*")
来源：http://llh.smart0.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wff.sufxvd.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bgm.fktsv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ihk.jianghu66.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kep.ydzc1.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zdq.yj202588.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wxw.hysaishi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uoq.jinqigfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mly.xylfe.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rfa.ivvv.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vap.zhiwuduotai.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://noi.9152youxi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://glh.hesvh.cn

[I07] 忽略大小写与多行模式
来源：http://tvx.bbcook.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ytk.hfpthk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mxc.tian-w.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ccf.jqgfzy.top

TS:   /error/gim
来源：http://gae.jinqigufen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ram.haohaochexian.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://van.feifeiyinyue.top

Ruby: s.scan(/error/i)
来源：http://uyf.iojbl.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qlb.sufxvd.cn

[I08] 贪婪与非贪婪匹配
来源：http://oko.bjfxy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nrt.hnqzz.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iqd.ehwqpu.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hck.bjfxy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://drh.andypj.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://ohr.daxiang520.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vpl.yuxming.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dob.jinqigfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xwg.epnwcf.com

================================================================================
来源：http://mdg.hywenlv.cn

J. 日期与时间
来源：http://emk.shuidangran.top

================================================================================
来源：http://ggp.pengpengdd.cyou

[J01] 获取当前时间
来源：http://qfo.yj20258.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://cjd.yanxiufei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ecy.jinqigfzy.top

JS:   new Date();  Date.now()
来源：http://eav.xziqi.cn

TS:   new Date();  Date.now()
来源：http://xiz.havefunace.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wab.zhoulong.xyz

Go:   time.Now()
来源：http://nad.yanxiufei.cn

Ruby: Time.now
来源：http://xhl.bbcook.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mhr.andypj.xyz

[J02] 格式化输出
来源：http://fje.quarkkingdee.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ndq.haohaochexian.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jvy.svipenyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ojv.zycfv.cn

TS:   d.toISOString()
来源：http://kbf.zdbjq.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://smz.jinqigfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mja.meibo888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fnb.fzhhl.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tgy.guowangkeji.top

[J03] 字符串解析为日期
来源：http://akz.jinyuanbaomall.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dpz.ydjk.org.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zsu.zhengqikj.top

JS:   new Date("2024-01-02")
来源：http://mes.yueranfly.top

TS:   new Date("2024-01-02")
来源：http://kqr.c1oappe.top

Java: LocalDate.parse("2024-01-02")
来源：http://jgq.xziqi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mic.gzhubu.top

Ruby: Date.parse("2024-01-02")
来源：http://bcn.chenzaomai.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jqz.hesvh.cn

[J04] 时间戳与日期互转
来源：http://lal.yuanzhike.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pzs.cheryme.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gzp.316326.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://azn.havefunace.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ifq.tianlin.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kqo.zdqjudy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vgb.meibo888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ado.haohaochexian.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bbw.hfpthk.cn

[J05] 时间加减（加 7 天）
来源：http://jlp.zhaomingkeji.xyz

Py:   now + timedelta(days=7)
来源：http://kmo.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://isx.gaohongyu789.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bfr.kuanghao11.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oux.jqgfzy.top

Java: LocalDate.now().plusDays(7)
来源：http://icz.nanxinkj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://feg.wangdashe.top

Ruby: Time.now + 7 * 86400
来源：http://rom.shangyingyoupin.top

C#:   DateTime.Now.AddDays(7)
来源：http://pyy.ywan-chungtsiang.top

[J06] 计算两时间之差
来源：http://ptf.yanxiufei.cn

Py:   (end - start).total_seconds()
来源：http://owa.yj20258888.top

PHP:  $end->diff($start)->days;
来源：http://lbs.tarul.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bpw.yfazqb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://reg.gogol.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rfh.ydjk.org.cn

Go:   end.Sub(start).Hours()
来源：http://ysa.wangshuangyany.cn

Ruby: end - start                 # 返回秒数
来源：http://dgb.9152youxi.cn

C#:   (end - start).TotalSeconds
来源：http://cli.daxiang520.top

[J07] 比较两个日期
来源：http://ore.quarkkingdee.top

Py:   d1 < d2;  d1 == d2
来源：http://ekp.xinyue.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uaz.gzhubu.top

JS:   d1.getTime() < d2.getTime()
来源：http://gio.hnqzz.top

TS:   d1.getTime() < d2.getTime()
来源：http://dmj.sxryk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://iyn.fzhhl.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tiw.cdnleiting.top

Ruby: d1 < d2;  d1 == d2
来源：http://xki.ybcxt.top

C#:   d1 < d2;  d1 == d2
来源：http://kip.hnxiangtu.top

[J08] 提取年月日与星期
来源：http://evg.c1oappe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wxr.jqgfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ddx.316326.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dgl.hfpthk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vfs.iojbl.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://die.hcnkem.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jup.gzhubu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qch.jlsjyb.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://glz.zhoulong.xyz

[J09] 时区处理
来源：http://coj.xziqi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tiz.zhixingplan.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iou.xylfe.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eqi.ybcxt.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xoh.gzhubu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rka.fzhhl.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bxt.chenlongwang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ize.yuxming.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ygj.guowangkeji.top

[J10] 取今天 / 本月第一天
来源：http://xix.yuxming.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uqj.zhaomingkeji.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qny.smart0.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tnq.bbcook.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tmy.hfpthk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mcv.zycfv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://amj.meibo888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iad.fzhhl.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ozl.wangshuangyany.cn

================================================================================
来源：http://bqw.fengsongda.top

K. JSON 与序列化
来源：http://dcl.zhengqikj.top

================================================================================
来源：http://vch.ydjk.org.cn

[K01] 对象转 JSON 字符串
来源：http://xcr.yueranfly.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rgo.hongshengwenyu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ctt.sxryk.cn

JS:   JSON.stringify(obj)
来源：http://fza.sufxvd.cn

TS:   JSON.stringify(obj)
来源：http://leg.gaohongyu789.top


<!-- 参考信息 -->