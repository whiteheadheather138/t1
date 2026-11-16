代发 wailian999

Py:   isinstance(u, User)
来源：http://tmn.sufxvd.cn

PHP:  $u instanceof User
来源：http://msg.iojbl.cn

JS:   u instanceof User
来源：http://yca.xinyue.icu

TS:   u instanceof User
来源：http://znv.daria6918.cn

Java: u instanceof User
来源：http://xfr.fzhhl.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hkh.yuanzhike.top

Ruby: u.is_a?(User)
来源：http://pjx.meibo888.top

C#:   u is User
来源：http://rjn.chenjidiqi.icu

[G14] 数据类 / record
来源：http://ctv.sjlbkw.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blz.c1oappe.top

PHP:  // 用 readonly 属性模拟
来源：http://kgx.daria6918.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rpa.hongshengwenyu.top

TS:   type User = { name: string; age: number };
来源：http://trm.redwolf501.top

Java: record User(String name, int age) {}
来源：http://wfw.zhiwuduotai.top

Go:   type User struct { Name string; Age int }
来源：http://auo.zhaomingkeji.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nmi.ppjwa.cn

C#:   record User(string Name, int Age);
来源：http://hbk.ctjpmb.com

[G15] 枚举
来源：http://iuz.xylfe.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mph.sysykeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tve.chenjidiqi.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hap.daria6918.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ebi.bjfxy.top

Java: enum Color { RED, GREEN }
来源：http://lrs.chenjidiqi.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://huh.smart0.xyz

Ruby: Color = %i[red green].freeze
来源：http://hvn.zhengqikj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rso.haohaochexian.top

[G16] 对象转数组 / 字典
来源：http://qwz.ywan-chungtsiang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eas.52xcode.cn

PHP:  get_object_vars($obj);
来源：http://vly.zdbjq.cn

JS:   Object.entries(obj)
来源：http://vln.gogol.net.cn

TS:   Object.entries(obj)
来源：http://lbg.shuidangran.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sbu.zhongyouzk.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ara.yj202588.top

Ruby: obj.instance_variables
来源：http://tgg.smart0.xyz

C#:   // 用反射或 System.Text.Json
来源：http://qoj.tianlin.xyz

================================================================================
来源：http://ufh.redwolf501.top

H. 异常与错误处理
来源：http://cnj.zhaomingkeji.xyz

================================================================================
来源：http://wgh.meibo888.top

[H01] try / catch 基础
来源：http://hlq.wangshuangyany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jym.yanxiufei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mdu.ydjk.org.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jlj.gzhubu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gxt.feifeiyinyue.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://odv.jyoumei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://orb.dashuyun.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uys.ydzc1.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ggx.aizwys.cn

[H02] finally / ensure 收尾
来源：http://ygr.sweek.top

Py:   try: f()⏎finally: cleanup()
来源：http://lfh.epnwcf.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://kvr.svipenyu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hbc.xinyue.icu

TS:   try { f(); } finally { cleanup(); }
来源：http://gez.ybcxt.top

Java: try { f(); } finally { cleanup(); }
来源：http://dgs.nwbrower.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://crl.yanxiufei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jjp.jianghu66.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xkq.sysykeji.top

[H03] 主动抛出异常
来源：http://ikb.tian-w.cn

Py:   raise ValueError("错误信息")
来源：http://kve.yvedp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sbc.epnwcf.com

JS:   throw new Error("错误信息");
来源：http://swz.mhx1999.top

TS:   throw new Error("错误信息");
来源：http://den.zdbjq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kue.jinqigufen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xdl.uphjek.com

Ruby: raise ArgumentError, "错误信息"
来源：http://dqs.hongshengwenyu.top

C#:   throw new ArgumentException("错误信息");
来源：http://ryw.fktsv.cn

[H04] 自定义异常类型
来源：http://uqj.fanxiaobao.xyz

Py:   class MyError(Exception): pass
来源：http://ylh.gotoacloud.top

PHP:  class MyError extends RuntimeException {}
来源：http://ifv.jlsjyb.cn

JS:   class MyError extends Error {}
来源：http://efu.guannengcc.top

TS:   class MyError extends Error {}
来源：http://pan.bbcook.cn

Java: class MyException extends RuntimeException {}
来源：http://pig.ivvv.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hvr.kuanghao11.cn

Ruby: class MyError < StandardError; end
来源：http://vdd.yuanzhike.top

C#:   class MyException : Exception {}
来源：http://yec.xziqi.cn

[H05] 捕获特定类型
来源：http://yxw.xuanzx.com

Py:   except ValueError as e:
来源：http://ozg.epnwcf.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zak.gotoacloud.top

JS:   if (e instanceof TypeError) {}
来源：http://zse.0kj1m.cn

TS:   if (e instanceof TypeError) {}
来源：http://fql.xingfuxueyuan.xyz

Java: catch (IOException | SQLException e) {}
来源：http://xce.haohaochexian.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rhl.hnqzz.top

Ruby: rescue ArgumentError => e
来源：http://pfd.zhongyouzk.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jxc.yuxming.cn

[H06] 可选值 / 空值安全访问
来源：http://xxx.zhongyouzk.top

Py:   value = d.get("k") or default
来源：http://haj.sxryk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jgy.fehbvm.com

JS:   obj?.a?.b;  d ?? default
来源：http://vzu.zhijiandao.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ouj.tarul.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lkp.tarul.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nap.bjfxy.top

Ruby: d&.dig(:a, :b)
来源：http://ahx.ydzc1.top

C#:   obj?.A?.B ?? default
来源：http://oyy.shangyingyoupin.top

[H07] 断言
来源：http://bgk.tarul.cn

Py:   assert x > 0, "必须为正"
来源：http://trf.quarkkingdee.top

PHP:  assert($x > 0);
来源：http://djw.yangfankeji.com

JS:   console.assert(x > 0);
来源：http://tyc.nanxinkj.top

TS:   console.assert(x > 0);
来源：http://qik.zhoulong.xyz

Java: assert x > 0 : "必须为正";
来源：http://jjj.cqqwz.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rix.fzhhl.top

Ruby: raise "必须为正" unless x > 0
来源：http://swq.jqgfzy.top

C#:   Debug.Assert(x > 0);
来源：http://ncl.aizwys.cn

[H08] 获取错误信息与堆栈
来源：http://lzy.zhongyouzk.top

Py:   str(e);  traceback.format_exc()
来源：http://aqj.cqqwz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://upc.jinqigufen.top

JS:   e.message;  e.stack
来源：http://iej.shzxlz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fbk.316326.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://pvr.vehdjk.com

Go:   err.Error()
来源：http://evm.jiagoushi.top

Ruby: e.message;  e.backtrace
来源：http://fkv.yj20258.top

C#:   e.Message;  e.StackTrace
来源：http://zwh.yj20258888.top

[H09] 带错误码的异常
来源：http://zoq.quarkkingdee.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://prv.uphjek.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://ooy.cdnleiting.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mak.mhx1999.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yyk.gzhubu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eon.gotoacloud.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://svr.iojbl.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rxv.xuetiantiany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qjq.ehwqpu.com

[H10] 资源自动释放
来源：http://fej.sweek.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ipd.zhijiandao.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://epj.ydjk.org.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gvg.hywenlv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uei.vqdsnc.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vbk.birdmap.top

Go:   defer f.Close()
来源：http://jtt.ehwqpu.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jjb.aibaodan.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fkn.yvedp.cn

================================================================================
来源：http://hto.vqdsnc.cn

I. 正则表达式
来源：http://dfm.xylfe.cn

================================================================================
来源：http://mhd.cdnleiting.top

[I01] 判断是否匹配
来源：http://lxc.pycfn.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://smb.fzhhl.top

PHP:  preg_match('/\d+/', $s);
来源：http://ixe.yvedp.cn

JS:   /\d+/.test(s)
来源：http://ive.guowangkeji.top

TS:   /\d+/.test(s)
来源：http://stm.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zto.smart0.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://phd.svipenyu.cn

Ruby: s.match?(/\d+/)
来源：http://him.shzxlz.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ukx.chenlongwang.top

[I02] 提取所有匹配
来源：http://aun.jiagoushi.top

Py:   re.findall(r"\d+", s)
来源：http://buq.hfpthk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ohs.jlsjyb.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gck.wangdashe.top

TS:   s.match(/\d+/g)
来源：http://zxs.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qje.xziqi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wvp.tanke756.top

Ruby: s.scan(/\d+/)
来源：http://aql.zhiwuduotai.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kvg.ydzc1.top

[I03] 提取捕获分组
来源：http://xmx.dashuyun.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jjd.daxiang520.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fln.shanyushiyangtech.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ceq.xinyue.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ivk.yangfankeji.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uer.yanxiufei.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qrn.ydzc1.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dip.xylfe.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iie.iojbl.cn

[I04] 正则替换
来源：http://fez.smart0.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://hrp.shangyingyoupin.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uvl.sjlbkw.cn

JS:   s.replace(/\d+/g, "#")
来源：http://oyg.iojbl.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tjv.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://iix.yj20258888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dqj.aibaodan.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://doj.yueranfly.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zls.xuanzx.com

[I05] 按正则拆分
来源：http://uwp.jqgfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://sbu.shanyushiyangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rbz.jinyuanbaomall.cn

JS:   s.split(/\s*,\s*/)
来源：http://cvx.dashuyun.cn

TS:   s.split(/\s*,\s*/)
来源：http://rbh.9152youxi.cn

Java: s.split("\\s*,\\s*")
来源：http://qzq.jinqigfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://egw.daria6918.cn

Ruby: s.split(/\s*,\s*/)
来源：http://afg.sxryk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hzc.bjfxy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nuz.yj20258.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ynq.cashguo.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wyt.zhongyouzk.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ksn.ehwqpu.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kds.nanxuanxn.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://taa.aizwys.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ujc.zdqjudy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mwq.aibaodan.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jco.wangshuangyany.cn

[I07] 忽略大小写与多行模式
来源：http://jxy.wangshuangyany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qau.yvedp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://aat.xziqi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qkt.dashuyun.cn

TS:   /error/gim
来源：http://ynp.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mji.nwbrower.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yzb.guannengcc.top

Ruby: s.scan(/error/i)
来源：http://gqe.gzhubu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qhl.ppjwa.cn

[I08] 贪婪与非贪婪匹配
来源：http://oqk.yj20258.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kas.nanxinkj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zmk.c1oappe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dfz.yuxming.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qlh.cqqwz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gtx.vehdjk.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bwi.jiagoushi.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://egu.fengsongda.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wib.fengsongda.top

================================================================================
来源：http://xzh.tarul.cn

J. 日期与时间
来源：http://xcb.tianlin.xyz

================================================================================
来源：http://cxt.jinqigfzy.top

[J01] 获取当前时间
来源：http://fvh.shangyingyoupin.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nwq.c1oappe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zmu.9152youxi.cn

JS:   new Date();  Date.now()
来源：http://riq.bjfxy.top

TS:   new Date();  Date.now()
来源：http://yym.vehdjk.com

Java: LocalDateTime.now();  Instant.now()
来源：http://bzj.xziqi.cn

Go:   time.Now()
来源：http://fhr.bjfxy.top

Ruby: Time.now
来源：http://aox.cucudq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rof.jinqigufen.top

[J02] 格式化输出
来源：http://frm.vqdsnc.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gmd.fengsongda.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://paz.zhengqikj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://drc.zhoulong.xyz

TS:   d.toISOString()
来源：http://iow.hysaishi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mot.daria6918.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://elf.ydzc1.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uti.svipenyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fay.pengpengdd.cyou

[J03] 字符串解析为日期
来源：http://wpp.zhoulong.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ypn.cashguo.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xze.dianchejie.cn

JS:   new Date("2024-01-02")
来源：http://tan.jqgufenzy.top

TS:   new Date("2024-01-02")
来源：http://whb.wangshuangyany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yok.jinghuilouyu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rgs.aibaodan.cn

Ruby: Date.parse("2024-01-02")
来源：http://vrd.gotoacloud.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://klg.aizwys.cn

[J04] 时间戳与日期互转
来源：http://ipt.andypj.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://loa.fanxiaobao.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://idy.nwbrower.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://knz.hysaishi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lvh.shangyingyoupin.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zkd.bjfxy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ela.yj202588.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://msa.fanxiaobao.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tuw.shanyushiyangkeji.top

[J05] 时间加减（加 7 天）
来源：http://jej.bbcook.cn

Py:   now + timedelta(days=7)
来源：http://qbt.epnwcf.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://dsh.mhx1999.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zej.aibaodan.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://apk.xziqi.cn

Java: LocalDate.now().plusDays(7)
来源：http://mrq.feifeiyinyue.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jrd.cdnleiting.top

Ruby: Time.now + 7 * 86400
来源：http://njx.hammf.cn

C#:   DateTime.Now.AddDays(7)
来源：http://csv.bbcook.cn

[J06] 计算两时间之差
来源：http://ens.chenzaomai.com

Py:   (end - start).total_seconds()
来源：http://oxp.bbcook.cn

PHP:  $end->diff($start)->days;
来源：http://zqi.cqqwz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oxf.hcnkem.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zsv.sweek.top

Java: Duration.between(start, end).toSeconds()
来源：http://fxg.dashuyun.cn

Go:   end.Sub(start).Hours()
来源：http://qxu.zhengqikj.top

Ruby: end - start                 # 返回秒数
来源：http://ylr.hcnkem.com

C#:   (end - start).TotalSeconds
来源：http://dju.pycfn.com

[J07] 比较两个日期
来源：http://swn.chenzaomai.com

Py:   d1 < d2;  d1 == d2
来源：http://wzr.cqqwz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vbz.ydzc1.top

JS:   d1.getTime() < d2.getTime()
来源：http://bwb.yanxiufei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xjw.mhx1999.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dvs.xuanzx.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qfa.chenlongwang.top

Ruby: d1 < d2;  d1 == d2
来源：http://kxr.bbcook.cn

C#:   d1 < d2;  d1 == d2
来源：http://yqe.hnqzz.top

[J08] 提取年月日与星期
来源：http://kfb.yfazqb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iwm.hnqzz.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bjr.andypj.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vgc.c1oappe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ibs.cheryme.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gwg.sufxvd.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dfc.jyoumei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oge.dianchejie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wjw.dianchejie.cn

[J09] 时区处理
来源：http://udp.c1oappe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kck.quarkkingdee.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://txy.jiagoushi.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kbx.wangdashe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ibr.haohaochexian.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://flv.gzhubu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gvd.hysaishi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ghk.meibo888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zaw.yanxiufei.cn

[J10] 取今天 / 本月第一天
来源：http://enj.mhx1999.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ysq.yonumen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://euw.cashguo.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zws.aizwys.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xyl.jqgufenzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gch.redwolf501.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wyj.zhaomingkeji.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dwc.zhaomingkeji.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lar.xuetiantiany.cn

================================================================================
来源：http://tba.jinyuanbaomall.cn

K. JSON 与序列化
来源：http://ogd.jinyuanbaomall.cn

================================================================================
来源：http://jnb.sweek.top

[K01] 对象转 JSON 字符串
来源：http://dnl.havefunace.top


<!-- 参考信息 -->