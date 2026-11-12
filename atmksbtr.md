代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://mvp.zdbjq.cn

Ruby: def to_s; @name; end
来源：http://jlf.aizwys.cn

C#:   public override string ToString() => Name;
来源：http://per.guowangkeji.top

[G13] 判断对象类型
来源：http://tge.jlsjyb.cn

Py:   isinstance(u, User)
来源：http://nsl.xinyue.icu

PHP:  $u instanceof User
来源：http://kuw.xuetiantiany.cn

JS:   u instanceof User
来源：http://yzb.yueranfly.top

TS:   u instanceof User
来源：http://ppa.yueranfly.top

Java: u instanceof User
来源：http://zkc.iojbl.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zxo.chenzaomai.com

Ruby: u.is_a?(User)
来源：http://ljv.jiagoushi.top

C#:   u is User
来源：http://rdh.yuxming.cn

[G14] 数据类 / record
来源：http://cin.fktsv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uwk.yj20258888.top

PHP:  // 用 readonly 属性模拟
来源：http://tsy.52xcode.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uwg.fengsongda.top

TS:   type User = { name: string; age: number };
来源：http://oro.chenlongwang.top

Java: record User(String name, int age) {}
来源：http://vet.uphjek.com

Go:   type User struct { Name string; Age int }
来源：http://anh.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ngd.sufxvd.cn

C#:   record User(string Name, int Age);
来源：http://ylg.guowangkeji.top

[G15] 枚举
来源：http://kip.gaohongyu789.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tku.hnqzz.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gwn.hesvh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bpl.fengsongda.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bxb.xylfe.cn

Java: enum Color { RED, GREEN }
来源：http://tkg.gzhubu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wfm.ydjk.org.cn

Ruby: Color = %i[red green].freeze
来源：http://njl.nwbrower.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rio.kuanghao11.cn

[G16] 对象转数组 / 字典
来源：http://hdy.fktsv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rnl.jqgfzy.top

PHP:  get_object_vars($obj);
来源：http://qys.dashuyun.cn

JS:   Object.entries(obj)
来源：http://ywi.shanyushiyangtech.top

TS:   Object.entries(obj)
来源：http://yzd.mhx1999.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hob.andypj.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://dtr.316326.xyz

Ruby: obj.instance_variables
来源：http://jjy.quarkkingdee.top

C#:   // 用反射或 System.Text.Json
来源：http://msc.wangshuangyany.cn

================================================================================
来源：http://uid.havefunace.top

H. 异常与错误处理
来源：http://tnh.nwbrower.top

================================================================================
来源：http://cid.daxiang520.top

[H01] try / catch 基础
来源：http://onm.yvedp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vsw.jianghu66.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://biu.meibo888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mxk.c1oappe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hqy.316326.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://idm.52xcode.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xwr.gaohongyu789.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://boe.fanxiaobao.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://utu.pycfn.com

[H02] finally / ensure 收尾
来源：http://stl.vehdjk.com

Py:   try: f()⏎finally: cleanup()
来源：http://vyu.zhoulong.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://bha.aizwys.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cjs.gogol.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fzx.hcnkem.com

Java: try { f(); } finally { cleanup(); }
来源：http://lph.zhiwuduotai.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wfn.cqqwz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cet.sxryk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zfc.aibaodan.cn

[H03] 主动抛出异常
来源：http://jmc.chenjidiqi.icu

Py:   raise ValueError("错误信息")
来源：http://jkw.cqqwz.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pmu.jlsjyb.cn

JS:   throw new Error("错误信息");
来源：http://flz.dashuyun.cn

TS:   throw new Error("错误信息");
来源：http://qeo.hammf.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bsj.cqqwz.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hkv.xuanzx.com

Ruby: raise ArgumentError, "错误信息"
来源：http://oly.gotoacloud.top

C#:   throw new ArgumentException("错误信息");
来源：http://aiv.ydzc1.top

[H04] 自定义异常类型
来源：http://jks.bjfxy.top

Py:   class MyError(Exception): pass
来源：http://chp.daria6918.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mpu.tianlin.xyz

JS:   class MyError extends Error {}
来源：http://sfv.bjfxy.top

TS:   class MyError extends Error {}
来源：http://tbh.zdbjq.cn

Java: class MyException extends RuntimeException {}
来源：http://qwk.xuanzx.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fyh.ybcxt.top

Ruby: class MyError < StandardError; end
来源：http://wrf.xuanzx.com

C#:   class MyException : Exception {}
来源：http://lgu.pengpengdd.cyou

[H05] 捕获特定类型
来源：http://rtb.zhongyouzk.top

Py:   except ValueError as e:
来源：http://snw.hammf.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dye.ywan-chungtsiang.top

JS:   if (e instanceof TypeError) {}
来源：http://ici.smart0.xyz

TS:   if (e instanceof TypeError) {}
来源：http://pmk.shzxlz.cn

Java: catch (IOException | SQLException e) {}
来源：http://aih.c1oappe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ofk.zhaomingkeji.xyz

Ruby: rescue ArgumentError => e
来源：http://hez.tarul.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://neq.chenzaomai.com

[H06] 可选值 / 空值安全访问
来源：http://sqz.jinyuanbaomall.cn

Py:   value = d.get("k") or default
来源：http://dds.ctjpmb.com

PHP:  $v = $d["k"] ?? null;
来源：http://fdw.quarkkingdee.top

JS:   obj?.a?.b;  d ?? default
来源：http://hiv.9152youxi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://oqk.c1oappe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ldb.jqgfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://pis.cdnleiting.top

Ruby: d&.dig(:a, :b)
来源：http://xem.xinyue.icu

C#:   obj?.A?.B ?? default
来源：http://cjn.ybcxt.top

[H07] 断言
来源：http://kci.gotoacloud.top

Py:   assert x > 0, "必须为正"
来源：http://sob.ivvv.top

PHP:  assert($x > 0);
来源：http://efa.dianchejie.cn

JS:   console.assert(x > 0);
来源：http://vav.fengsongda.top

TS:   console.assert(x > 0);
来源：http://kxc.52xcode.cn

Java: assert x > 0 : "必须为正";
来源：http://abh.jqgfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wgb.shangyingyoupin.top

Ruby: raise "必须为正" unless x > 0
来源：http://bws.dashuyun.cn

C#:   Debug.Assert(x > 0);
来源：http://ozk.shanyushiyangtech.top

[H08] 获取错误信息与堆栈
来源：http://xvb.yj20258.top

Py:   str(e);  traceback.format_exc()
来源：http://kfh.cashguo.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ibu.zhengqikj.top

JS:   e.message;  e.stack
来源：http://pyk.dianchejie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hkp.ppjwa.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://haa.yangfankeji.com

Go:   err.Error()
来源：http://gds.meibo888.top

Ruby: e.message;  e.backtrace
来源：http://eee.pengpengdd.cyou

C#:   e.Message;  e.StackTrace
来源：http://twp.cdnleiting.top

[H09] 带错误码的异常
来源：http://cec.redwolf501.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kiq.guannengcc.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://uqm.fengsongda.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xif.ctjpmb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bno.feifeiyinyue.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wef.wangshuangyany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kzb.xziqi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sbt.ywan-chungtsiang.top

C#:   // 自定义异常类中加 Code 属性
来源：http://uke.wangdashe.top

[H10] 资源自动释放
来源：http://jen.ivvv.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://coc.jyoumei.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xhc.yj20258888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tjf.dianchejie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jmk.316326.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xag.guannengcc.top

Go:   defer f.Close()
来源：http://oyf.hywenlv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hgy.havefunace.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ulb.nanxuanxn.top

================================================================================
来源：http://lls.cqqwz.cn

I. 正则表达式
来源：http://ocd.ydjk.org.cn

================================================================================
来源：http://doj.svipenyu.cn

[I01] 判断是否匹配
来源：http://wsf.zhongyouzk.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nln.hfpthk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vlv.daria6918.cn

JS:   /\d+/.test(s)
来源：http://aad.pycfn.com

TS:   /\d+/.test(s)
来源：http://trj.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qhq.epnwcf.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nzu.nwbrower.top

Ruby: s.match?(/\d+/)
来源：http://fgy.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mzx.ydjk.org.cn

[I02] 提取所有匹配
来源：http://dyi.zycfv.cn

Py:   re.findall(r"\d+", s)
来源：http://hab.zdbjq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iah.yuxming.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ezj.ppjwa.cn

TS:   s.match(/\d+/g)
来源：http://tmi.bjfxy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vqt.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://eto.aizwys.cn

Ruby: s.scan(/\d+/)
来源：http://uly.fanxiaobao.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rpc.gaohongyu789.top

[I03] 提取捕获分组
来源：http://kni.cashguo.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hfe.svipenyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rtu.bjfxy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://adt.ivvv.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gpo.tian-w.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rmm.pengpengdd.cyou

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ckw.zhongyouzk.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://puu.pycfn.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://joi.hysaishi.cn

[I04] 正则替换
来源：http://btl.nanxuanxn.top

Py:   re.sub(r"\d+", "#", s)
来源：http://kzw.shanyushiyangtech.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xvb.aibaodan.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xhe.zhengqikj.top

TS:   s.replace(/\d+/g, "#")
来源：http://whd.havefunace.top

Java: s.replaceAll("\\d+", "#")
来源：http://sye.zhijiandao.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lmk.vqdsnc.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://oiu.feifeiyinyue.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tih.jinghuilouyu.cn

[I05] 按正则拆分
来源：http://rpv.fzhhl.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hhv.jinghuilouyu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tzg.cdnleiting.top

JS:   s.split(/\s*,\s*/)
来源：http://ncm.epnwcf.com

TS:   s.split(/\s*,\s*/)
来源：http://keo.zhixingplan.top

Java: s.split("\\s*,\\s*")
来源：http://blj.aibaodan.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mhd.daria6918.cn

Ruby: s.split(/\s*,\s*/)
来源：http://abd.shzxlz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xgs.ydzc1.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iva.jqgfzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dpr.dianchejie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gfa.xinyue.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pfv.ybcxt.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jac.xingfuxueyuan.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uid.pengpengdd.cyou

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://huo.xuanzx.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yrx.ppjwa.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jdx.yueranfly.top

[I07] 忽略大小写与多行模式
来源：http://hvx.aibaodan.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bhl.ybcxt.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lml.yvedp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rli.52xcode.cn

TS:   /error/gim
来源：http://wvj.andypj.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://iov.feifeiyinyue.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kyu.jinghuilouyu.cn

Ruby: s.scan(/error/i)
来源：http://vun.zhiwuduotai.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iwx.zhoulong.xyz

[I08] 贪婪与非贪婪匹配
来源：http://kwx.zhixingplan.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vlt.zhixingplan.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hzv.wangshuangyany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jvb.uphjek.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eqs.daria6918.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dkj.xuanzx.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eaw.cashguo.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rwv.pycfn.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://egg.tian-w.cn

================================================================================
来源：http://vsa.jinyuanbaomall.cn

J. 日期与时间
来源：http://yqi.redwolf501.top

================================================================================
来源：http://kjg.zdbjq.cn

[J01] 获取当前时间
来源：http://akf.aizwys.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bvx.sjlbkw.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vuf.daxiang520.top

JS:   new Date();  Date.now()
来源：http://aky.xziqi.cn

TS:   new Date();  Date.now()
来源：http://fgz.shanyushiyangtech.top

Java: LocalDateTime.now();  Instant.now()
来源：http://xzk.ybcxt.top

Go:   time.Now()
来源：http://wts.jinghuilouyu.cn

Ruby: Time.now
来源：http://rif.xuetiantiany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dcr.vehdjk.com

[J02] 格式化输出
来源：http://bdp.hnqzz.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hda.0kj1m.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://myx.chenzaomai.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ock.cucudq.cn

TS:   d.toISOString()
来源：http://jrb.dianchejie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ods.kuanghao11.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://djf.meibo888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xjp.ctjpmb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oyw.jinqigufen.top

[J03] 字符串解析为日期
来源：http://cit.yanxiufei.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://aec.jyoumei.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rdu.jlsjyb.cn

JS:   new Date("2024-01-02")
来源：http://fmz.tanke756.top

TS:   new Date("2024-01-02")
来源：http://sna.guannengcc.top

Java: LocalDate.parse("2024-01-02")
来源：http://xew.tanke756.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pmp.redwolf501.top

Ruby: Date.parse("2024-01-02")
来源：http://odr.gzhubu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rwb.yj20258888.top

[J04] 时间戳与日期互转
来源：http://faq.pycfn.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://udt.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vru.hfpthk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://apw.fanxiaobao.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://avt.gzhubu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wzh.chenzaomai.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jnz.dianchejie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vkc.wangdashe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kqa.aibaodan.cn

[J05] 时间加减（加 7 天）
来源：http://kax.ehwqpu.com

Py:   now + timedelta(days=7)
来源：http://uzx.hammf.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jdi.gogol.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://awa.ydjk.org.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://coq.tianlin.xyz

Java: LocalDate.now().plusDays(7)
来源：http://yap.cucudq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uwr.redwolf501.top

Ruby: Time.now + 7 * 86400
来源：http://hug.shanyushiyangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://bjw.yfazqb.com

[J06] 计算两时间之差
来源：http://ohf.yanxiufei.cn

Py:   (end - start).total_seconds()
来源：http://roz.smart0.xyz

PHP:  $end->diff($start)->days;
来源：http://eyh.wangdashe.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tkp.zycfv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kjn.feifeiyinyue.top

Java: Duration.between(start, end).toSeconds()
来源：http://tpj.tanke756.top

Go:   end.Sub(start).Hours()
来源：http://bnt.nanxuanxn.top

Ruby: end - start                 # 返回秒数
来源：http://qco.zhoulong.xyz

C#:   (end - start).TotalSeconds
来源：http://yeg.hfpthk.cn

[J07] 比较两个日期
来源：http://zun.jianghu66.top

Py:   d1 < d2;  d1 == d2
来源：http://rej.yfazqb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rbl.vehdjk.com

JS:   d1.getTime() < d2.getTime()
来源：http://qzo.nanxinkj.top

TS:   d1.getTime() < d2.getTime()
来源：http://rco.smart0.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lgf.yueranfly.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://emg.ywan-chungtsiang.top

Ruby: d1 < d2;  d1 == d2
来源：http://tgx.xuanzx.com

C#:   d1 < d2;  d1 == d2
来源：http://phj.gogol.net.cn

[J08] 提取年月日与星期
来源：http://rku.xylfe.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xpm.sysykeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ecr.zhaomingkeji.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mym.ivvv.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mpl.tarul.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sig.0kj1m.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://day.tanke756.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hkr.bbcook.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bev.shangyingyoupin.top

[J09] 时区处理
来源：http://sce.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tfq.yongpay.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cki.9152youxi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mlp.chenlongwang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://res.jianghu66.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nna.quarkkingdee.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://whk.jqgfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://tph.tanke756.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ryp.epnwcf.com

[J10] 取今天 / 本月第一天
来源：http://qgg.xingfuxueyuan.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://upz.wangshuangyany.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://drc.ybcxt.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uqt.zhoulong.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uqr.hfpthk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jww.yj202588.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gif.quarkkingdee.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fel.gogol.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fcf.shuidangran.top


<!-- 参考信息 -->