代发 wailian999

Java: u instanceof User
来源：http://mok.zhiwuduotai.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ptp.chenlongwang.top

Ruby: u.is_a?(User)
来源：http://lhz.ybcxt.top

C#:   u is User
来源：http://nuf.sysykeji.top

[G14] 数据类 / record
来源：http://xes.uphjek.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qkl.hnxiangtu.top

PHP:  // 用 readonly 属性模拟
来源：http://cqi.gogol.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dvv.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://khb.hesvh.cn

Java: record User(String name, int age) {}
来源：http://udh.dianchejie.cn

Go:   type User struct { Name string; Age int }
来源：http://jlo.c1oappe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uso.tanke756.top

C#:   record User(string Name, int Age);
来源：http://inj.chenjidiqi.icu

[G15] 枚举
来源：http://lzt.hnqzz.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ptc.feifeiyinyue.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qve.yj20258888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cov.xylfe.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://whq.xinyue.icu

Java: enum Color { RED, GREEN }
来源：http://gyf.snrcjt.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kdh.pengpengdd.cyou

Ruby: Color = %i[red green].freeze
来源：http://zbo.yonumen.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://juz.shanyushiyangkeji.top

[G16] 对象转数组 / 字典
来源：http://dki.cheryme.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://onq.316326.xyz

PHP:  get_object_vars($obj);
来源：http://zms.zhixingplan.top

JS:   Object.entries(obj)
来源：http://xpd.fanxiaobao.xyz

TS:   Object.entries(obj)
来源：http://hkz.ppjwa.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://laz.cheryme.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ige.snrcjt.cn

Ruby: obj.instance_variables
来源：http://kyb.zhiwuduotai.top

C#:   // 用反射或 System.Text.Json
来源：http://dpc.jiagoushi.top

================================================================================
来源：http://mub.jinyuanbaomall.cn

H. 异常与错误处理
来源：http://pip.ivvv.top

================================================================================
来源：http://jfo.zdbjq.cn

[H01] try / catch 基础
来源：http://noc.nanxuanxn.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vhn.jqgufenzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gmr.uphjek.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hev.zycfv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tjf.hesvh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ikq.ybcxt.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hhj.gaohongyu789.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://saw.mhx1999.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bio.yueranfly.top

[H02] finally / ensure 收尾
来源：http://wwb.nwbrower.top

Py:   try: f()⏎finally: cleanup()
来源：http://ilo.yfazqb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://lgr.shanyushiyangtech.top

JS:   try { f(); } finally { cleanup(); }
来源：http://biu.bbcook.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oek.cashguo.top

Java: try { f(); } finally { cleanup(); }
来源：http://vnp.jyoumei.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rid.hesvh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wgr.ydzc1.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pox.smart0.xyz

[H03] 主动抛出异常
来源：http://mtn.jlsjyb.cn

Py:   raise ValueError("错误信息")
来源：http://pou.uphjek.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jnl.hfpthk.cn

JS:   throw new Error("错误信息");
来源：http://rrt.smart0.xyz

TS:   throw new Error("错误信息");
来源：http://ntn.jianghu66.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hle.fengsongda.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mza.dashuyun.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cdm.feifeiyinyue.top

C#:   throw new ArgumentException("错误信息");
来源：http://pwc.yuanzhike.top

[H04] 自定义异常类型
来源：http://eyf.xuanzx.com

Py:   class MyError(Exception): pass
来源：http://jqj.hnxiangtu.top

PHP:  class MyError extends RuntimeException {}
来源：http://ldd.yuxming.cn

JS:   class MyError extends Error {}
来源：http://pky.wangshuangyany.cn

TS:   class MyError extends Error {}
来源：http://xqd.ppjwa.cn

Java: class MyException extends RuntimeException {}
来源：http://guu.xziqi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xso.ybcxt.top

Ruby: class MyError < StandardError; end
来源：http://pnl.hnxiangtu.top

C#:   class MyException : Exception {}
来源：http://ugf.andypj.xyz

[H05] 捕获特定类型
来源：http://hqs.gotoacloud.top

Py:   except ValueError as e:
来源：http://ebk.sufxvd.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://orf.redwolf501.top

JS:   if (e instanceof TypeError) {}
来源：http://lid.xuetiantiany.cn

TS:   if (e instanceof TypeError) {}
来源：http://sev.iojbl.cn

Java: catch (IOException | SQLException e) {}
来源：http://hpb.yuanzhike.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vfk.epnwcf.com

Ruby: rescue ArgumentError => e
来源：http://nus.chenjidiqi.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ind.yuxming.cn

[H06] 可选值 / 空值安全访问
来源：http://ygj.yuxming.cn

Py:   value = d.get("k") or default
来源：http://nve.mhx1999.top

PHP:  $v = $d["k"] ?? null;
来源：http://dab.ehwqpu.com

JS:   obj?.a?.b;  d ?? default
来源：http://jqa.fengsongda.top

TS:   obj?.a?.b;  d ?? default
来源：http://ltl.jinyuanbaomall.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ecn.hywenlv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fxw.9152youxi.cn

Ruby: d&.dig(:a, :b)
来源：http://laz.wangshuangyany.cn

C#:   obj?.A?.B ?? default
来源：http://tou.yueranfly.top

[H07] 断言
来源：http://acd.zhijiandao.cn

Py:   assert x > 0, "必须为正"
来源：http://clk.ybcxt.top

PHP:  assert($x > 0);
来源：http://zld.daria6918.cn

JS:   console.assert(x > 0);
来源：http://mgh.wangshuangyany.cn

TS:   console.assert(x > 0);
来源：http://gra.ydzc1.top

Java: assert x > 0 : "必须为正";
来源：http://lms.snrcjt.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cgg.jqgfzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://fqh.birdmap.top

C#:   Debug.Assert(x > 0);
来源：http://hpx.jqgfzy.top

[H08] 获取错误信息与堆栈
来源：http://dsv.fzhhl.top

Py:   str(e);  traceback.format_exc()
来源：http://ise.nanxinkj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mal.wangshuangyany.cn

JS:   e.message;  e.stack
来源：http://ejc.daxiang520.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ewb.daria6918.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fvl.pengpengdd.cyou

Go:   err.Error()
来源：http://tlb.xinyue.icu

Ruby: e.message;  e.backtrace
来源：http://luy.zhengqikj.top

C#:   e.Message;  e.StackTrace
来源：http://qkf.fzhhl.top

[H09] 带错误码的异常
来源：http://lui.tanke756.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oke.havefunace.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://bmy.snrcjt.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://taj.xingfuxueyuan.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dko.snrcjt.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yih.cqqwz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fss.zycfv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ojl.pycfn.com

C#:   // 自定义异常类中加 Code 属性
来源：http://yld.shzxlz.cn

[H10] 资源自动释放
来源：http://piz.ydzc1.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ghu.zhengqikj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bxb.sufxvd.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cld.shanyushiyangtech.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hec.wangdashe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xkg.cucudq.cn

Go:   defer f.Close()
来源：http://ipl.52xcode.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hqa.shzxlz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qwz.zdqjudy.top

================================================================================
来源：http://etp.yj20258.top

I. 正则表达式
来源：http://jtv.wangshuangyany.cn

================================================================================
来源：http://brg.gaohongyu789.top

[I01] 判断是否匹配
来源：http://mow.aibaodan.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ajr.jinqigfzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://lce.gogol.net.cn

JS:   /\d+/.test(s)
来源：http://qjw.shuidangran.top

TS:   /\d+/.test(s)
来源：http://eez.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pdb.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cgc.yuxming.cn

Ruby: s.match?(/\d+/)
来源：http://wsa.nanxuanxn.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lua.yfazqb.com

[I02] 提取所有匹配
来源：http://mat.shuidangran.top

Py:   re.findall(r"\d+", s)
来源：http://slg.shzxlz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://doo.yueranfly.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://upj.wangshuangyany.cn

TS:   s.match(/\d+/g)
来源：http://fms.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vfj.xziqi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vkm.0kj1m.cn

Ruby: s.scan(/\d+/)
来源：http://pup.sweek.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ifu.nanxuanxn.top

[I03] 提取捕获分组
来源：http://kxx.sxryk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dwz.316326.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lbo.fehbvm.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ajv.jqgufenzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://brc.52xcode.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xyv.zhaomingkeji.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wbd.ydzc1.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rpj.jiagoushi.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tsn.ctjpmb.com

[I04] 正则替换
来源：http://ign.hywenlv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zgz.zhoulong.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vcj.ivvv.top

JS:   s.replace(/\d+/g, "#")
来源：http://oed.mhx1999.top

TS:   s.replace(/\d+/g, "#")
来源：http://lxv.chenlongwang.top

Java: s.replaceAll("\\d+", "#")
来源：http://tka.chenlongwang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wvl.zhijiandao.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kec.jyoumei.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wpo.daxiang520.top

[I05] 按正则拆分
来源：http://hmo.jyoumei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fut.iojbl.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pip.fanxiaobao.xyz

JS:   s.split(/\s*,\s*/)
来源：http://ywr.shangyingyoupin.top

TS:   s.split(/\s*,\s*/)
来源：http://bae.sxryk.cn

Java: s.split("\\s*,\\s*")
来源：http://oui.jinghuilouyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lac.zdqjudy.top

Ruby: s.split(/\s*,\s*/)
来源：http://vxi.hongshengwenyu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lod.quarkkingdee.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lel.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wdz.yuxming.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ium.xinyue.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://olg.gotoacloud.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ynn.hcnkem.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zpp.9152youxi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vbc.hcnkem.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uuo.c1oappe.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xhb.andypj.xyz

[I07] 忽略大小写与多行模式
来源：http://ufc.daxiang520.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qxi.xingfuxueyuan.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nyq.meibo888.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dkv.ydjk.org.cn

TS:   /error/gim
来源：http://wkx.ppjwa.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jcy.feifeiyinyue.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kpb.xuetiantiany.cn

Ruby: s.scan(/error/i)
来源：http://olt.guannengcc.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zup.gzhubu.top

[I08] 贪婪与非贪婪匹配
来源：http://sul.hfpthk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mmk.shanyushiyangkeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://omh.haohaochexian.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://via.gaohongyu789.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fsq.dashuyun.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xhc.redwolf501.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vns.kuanghao11.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ohy.cucudq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hcc.wangshuangyany.cn

================================================================================
来源：http://wfv.fktsv.cn

J. 日期与时间
来源：http://mec.yuxming.cn

================================================================================
来源：http://jxs.kuanghao11.cn

[J01] 获取当前时间
来源：http://pxj.zdqjudy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mrp.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wrd.zhengqikj.top

JS:   new Date();  Date.now()
来源：http://ipj.jinqigfzy.top

TS:   new Date();  Date.now()
来源：http://xvt.sxryk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fbt.feifeiyinyue.top

Go:   time.Now()
来源：http://fpy.fehbvm.com

Ruby: Time.now
来源：http://adc.fehbvm.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://onz.hesvh.cn

[J02] 格式化输出
来源：http://cxb.aizwys.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qox.smart0.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hub.gaohongyu789.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ixb.chenzaomai.com

TS:   d.toISOString()
来源：http://ngr.yueranfly.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yik.nanxuanxn.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tgk.xziqi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tfk.snrcjt.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vyw.xinyue.icu

[J03] 字符串解析为日期
来源：http://pdq.redwolf501.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wba.zhoulong.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uvm.tanke756.top

JS:   new Date("2024-01-02")
来源：http://yyq.haohaochexian.top

TS:   new Date("2024-01-02")
来源：http://qou.bbcook.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mua.guannengcc.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lap.zdqjudy.top

Ruby: Date.parse("2024-01-02")
来源：http://ehw.xinyue.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xch.shzxlz.cn

[J04] 时间戳与日期互转
来源：http://kqq.tian-w.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ubm.yuanzhike.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ung.ydzc1.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cac.ydjk.org.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jkp.nanxinkj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fjb.yj20258888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gsg.yvedp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eqa.kuanghao11.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vgm.tanke756.top

[J05] 时间加减（加 7 天）
来源：http://hrw.yangfankeji.com

Py:   now + timedelta(days=7)
来源：http://wai.jianghu66.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cik.cdnleiting.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tmn.gogol.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gsj.jiagoushi.top

Java: LocalDate.now().plusDays(7)
来源：http://syc.yfazqb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xxo.guowangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://tjo.zhoulong.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://njr.zhoulong.xyz

[J06] 计算两时间之差
来源：http://dzb.jlsjyb.cn

Py:   (end - start).total_seconds()
来源：http://sis.ppjwa.cn

PHP:  $end->diff($start)->days;
来源：http://iiz.yfazqb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tcz.gogol.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dfp.zycfv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vcd.pycfn.com

Go:   end.Sub(start).Hours()
来源：http://pru.daxiang520.top

Ruby: end - start                 # 返回秒数
来源：http://eht.vqdsnc.cn

C#:   (end - start).TotalSeconds
来源：http://lgf.yuxming.cn

[J07] 比较两个日期
来源：http://keh.hysaishi.cn

Py:   d1 < d2;  d1 == d2
来源：http://djz.yvedp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://llt.nwbrower.top

JS:   d1.getTime() < d2.getTime()
来源：http://tug.fktsv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://aat.dashuyun.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://woe.sufxvd.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://egf.vehdjk.com

Ruby: d1 < d2;  d1 == d2
来源：http://szc.zhoulong.xyz

C#:   d1 < d2;  d1 == d2
来源：http://zyp.dianchejie.cn

[J08] 提取年月日与星期
来源：http://xoi.hnqzz.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qen.guannengcc.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ajj.bjfxy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vwx.smart0.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mdn.yfazqb.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://brv.gogol.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kos.hysaishi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://knu.shanyushiyangtech.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://awz.zhongyouzk.top

[J09] 时区处理
来源：http://qfi.cdnleiting.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xza.yueranfly.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://snc.hesvh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vbl.daxiang520.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dxf.chenjidiqi.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sdq.hfpthk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eaz.sufxvd.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jwo.ppjwa.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gex.hywenlv.cn

[J10] 取今天 / 本月第一天
来源：http://rkn.xinyue.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://rcc.ydzc1.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vyx.haohaochexian.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xua.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wxw.mhx1999.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mld.yangfankeji.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gle.mhx1999.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jal.shangyingyoupin.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ufe.hongshengwenyu.top

================================================================================
来源：http://nfz.yj20258888.top

K. JSON 与序列化
来源：http://gyx.dashuyun.cn

================================================================================
来源：http://zcq.yonumen.top

[K01] 对象转 JSON 字符串
来源：http://tcp.hnxiangtu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xfs.jiagoushi.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mce.yuanzhike.top

JS:   JSON.stringify(obj)
来源：http://lcy.c1oappe.top

TS:   JSON.stringify(obj)
来源：http://xug.sufxvd.cn


<!-- 参考信息 -->