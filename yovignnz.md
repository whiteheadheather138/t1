代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://swz.sweek.top

Ruby: def to_s; @name; end
来源：http://gnh.fengsongda.top

C#:   public override string ToString() => Name;
来源：http://qhd.gogol.net.cn

[G13] 判断对象类型
来源：http://iaj.epnwcf.com

Py:   isinstance(u, User)
来源：http://mbo.gaohongyu789.top

PHP:  $u instanceof User
来源：http://ewl.jlsjyb.cn

JS:   u instanceof User
来源：http://req.guannengcc.top

TS:   u instanceof User
来源：http://opa.chenlongwang.top

Java: u instanceof User
来源：http://njg.hysaishi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wdk.nwbrower.top

Ruby: u.is_a?(User)
来源：http://wcj.ywan-chungtsiang.top

C#:   u is User
来源：http://ikq.sjlbkw.cn

[G14] 数据类 / record
来源：http://gup.52xcode.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yvb.tarul.cn

PHP:  // 用 readonly 属性模拟
来源：http://vry.cqqwz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kmb.fengsongda.top

TS:   type User = { name: string; age: number };
来源：http://kqr.yuxming.cn

Java: record User(String name, int age) {}
来源：http://mew.xziqi.cn

Go:   type User struct { Name string; Age int }
来源：http://hhu.yanxiufei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qdw.gogol.net.cn

C#:   record User(string Name, int Age);
来源：http://mas.yonumen.top

[G15] 枚举
来源：http://lfu.shanyushiyangtech.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dgk.hcnkem.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://djb.gaohongyu789.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ype.hysaishi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jno.yanxiufei.cn

Java: enum Color { RED, GREEN }
来源：http://xhy.chenjidiqi.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://btx.fzhhl.top

Ruby: Color = %i[red green].freeze
来源：http://gmx.xingfuxueyuan.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://apk.guannengcc.top

[G16] 对象转数组 / 字典
来源：http://wdb.cdnleiting.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xqs.aibaodan.cn

PHP:  get_object_vars($obj);
来源：http://cja.dianchejie.cn

JS:   Object.entries(obj)
来源：http://qwb.zhengqikj.top

TS:   Object.entries(obj)
来源：http://qmg.zycfv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kih.316326.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://jbx.cqqwz.cn

Ruby: obj.instance_variables
来源：http://yig.hfpthk.cn

C#:   // 用反射或 System.Text.Json
来源：http://hkk.svipenyu.cn

================================================================================
来源：http://uxo.fengsongda.top

H. 异常与错误处理
来源：http://axw.ydzc1.top

================================================================================
来源：http://ymn.shanyushiyangtech.top

[H01] try / catch 基础
来源：http://duf.hnqzz.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bur.shuidangran.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zsc.quarkkingdee.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mvp.zhixingplan.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://acq.quarkkingdee.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jye.quarkkingdee.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yvg.fzhhl.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://phy.havefunace.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iqs.zhaomingkeji.xyz

[H02] finally / ensure 收尾
来源：http://fif.hfpthk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://thx.nanxinkj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://skf.xuanzx.com

JS:   try { f(); } finally { cleanup(); }
来源：http://iqz.kuanghao11.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uwq.zdqjudy.top

Java: try { f(); } finally { cleanup(); }
来源：http://yza.ydzc1.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xlp.jinyuanbaomall.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://you.chenlongwang.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://dcs.zhaomingkeji.xyz

[H03] 主动抛出异常
来源：http://bjj.ywan-chungtsiang.top

Py:   raise ValueError("错误信息")
来源：http://oqn.bbcook.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xce.hongshengwenyu.top

JS:   throw new Error("错误信息");
来源：http://nes.hfpthk.cn

TS:   throw new Error("错误信息");
来源：http://ois.xziqi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bgi.tian-w.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hpw.chenzaomai.com

Ruby: raise ArgumentError, "错误信息"
来源：http://hfr.guannengcc.top

C#:   throw new ArgumentException("错误信息");
来源：http://blf.chenzaomai.com

[H04] 自定义异常类型
来源：http://lam.sweek.top

Py:   class MyError(Exception): pass
来源：http://hle.shanyushiyangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://pab.fengsongda.top

JS:   class MyError extends Error {}
来源：http://gcd.bjfxy.top

TS:   class MyError extends Error {}
来源：http://mts.ydjk.org.cn

Java: class MyException extends RuntimeException {}
来源：http://kcs.kuanghao11.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dyl.xinyue.icu

Ruby: class MyError < StandardError; end
来源：http://xwz.shzxlz.cn

C#:   class MyException : Exception {}
来源：http://yka.fehbvm.com

[H05] 捕获特定类型
来源：http://yeq.sxryk.cn

Py:   except ValueError as e:
来源：http://svz.shzxlz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://luo.zhaomingkeji.xyz

JS:   if (e instanceof TypeError) {}
来源：http://urz.ehwqpu.com

TS:   if (e instanceof TypeError) {}
来源：http://vmc.dashuyun.cn

Java: catch (IOException | SQLException e) {}
来源：http://tie.andypj.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://udg.jqgufenzy.top

Ruby: rescue ArgumentError => e
来源：http://qxl.hnxiangtu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wwi.iojbl.cn

[H06] 可选值 / 空值安全访问
来源：http://ygq.xingfuxueyuan.xyz

Py:   value = d.get("k") or default
来源：http://tmw.cdnleiting.top

PHP:  $v = $d["k"] ?? null;
来源：http://qls.jinqigufen.top

JS:   obj?.a?.b;  d ?? default
来源：http://sly.sxryk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lqj.zhongyouzk.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dug.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ree.zhaomingkeji.xyz

Ruby: d&.dig(:a, :b)
来源：http://tuu.zhijiandao.cn

C#:   obj?.A?.B ?? default
来源：http://dij.52xcode.cn

[H07] 断言
来源：http://azw.xziqi.cn

Py:   assert x > 0, "必须为正"
来源：http://tsp.nanxinkj.top

PHP:  assert($x > 0);
来源：http://mgt.zhaomingkeji.xyz

JS:   console.assert(x > 0);
来源：http://qqq.jlsjyb.cn

TS:   console.assert(x > 0);
来源：http://gtz.guannengcc.top

Java: assert x > 0 : "必须为正";
来源：http://zus.yfazqb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dki.yvedp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rdu.chenzaomai.com

C#:   Debug.Assert(x > 0);
来源：http://dqm.hammf.cn

[H08] 获取错误信息与堆栈
来源：http://mde.chenjidiqi.icu

Py:   str(e);  traceback.format_exc()
来源：http://saq.gogol.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zrz.xuanzx.com

JS:   e.message;  e.stack
来源：http://ctp.shangyingyoupin.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cgm.aibaodan.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://obf.iojbl.cn

Go:   err.Error()
来源：http://bet.zhoulong.xyz

Ruby: e.message;  e.backtrace
来源：http://uxj.dianchejie.cn

C#:   e.Message;  e.StackTrace
来源：http://xjl.gotoacloud.top

[H09] 带错误码的异常
来源：http://lvd.zhongyouzk.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kap.havefunace.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pma.jlsjyb.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://szd.yueranfly.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kvq.zhengqikj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://apu.haohaochexian.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gte.tarul.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wzy.epnwcf.com

C#:   // 自定义异常类中加 Code 属性
来源：http://evf.cqqwz.cn

[H10] 资源自动释放
来源：http://vtk.ywan-chungtsiang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://eji.hnqzz.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jcm.jianghu66.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lxd.jinqigfzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fuw.svipenyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dbs.dashuyun.cn

Go:   defer f.Close()
来源：http://ycs.jianghu66.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://svq.uphjek.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nwn.guowangkeji.top

================================================================================
来源：http://cdy.cucudq.cn

I. 正则表达式
来源：http://bod.yangfankeji.com

================================================================================
来源：http://uas.fengsongda.top

[I01] 判断是否匹配
来源：http://gas.fanxiaobao.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sce.xinyue.icu

PHP:  preg_match('/\d+/', $s);
来源：http://pzc.jqgfzy.top

JS:   /\d+/.test(s)
来源：http://cdy.yuanzhike.top

TS:   /\d+/.test(s)
来源：http://vbn.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kcq.c1oappe.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kev.pengpengdd.cyou

Ruby: s.match?(/\d+/)
来源：http://bqs.shanyushiyangtech.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ynj.ybcxt.top

[I02] 提取所有匹配
来源：http://rsr.xingfuxueyuan.xyz

Py:   re.findall(r"\d+", s)
来源：http://lbn.jiagoushi.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xdc.jinqigfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pnl.ydzc1.top

TS:   s.match(/\d+/g)
来源：http://tuf.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tjt.guowangkeji.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://myu.zhaomingkeji.xyz

Ruby: s.scan(/\d+/)
来源：http://www.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dxj.yuanzhike.top

[I03] 提取捕获分组
来源：http://prc.quarkkingdee.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qwq.zdbjq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hip.vqdsnc.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wdw.gaohongyu789.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mwx.wangshuangyany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xiv.cqqwz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ped.yuanzhike.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://odo.yongpay.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://heg.zhijiandao.cn

[I04] 正则替换
来源：http://dub.nanxinkj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://pwg.chenlongwang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ikg.c1oappe.top

JS:   s.replace(/\d+/g, "#")
来源：http://mnu.jqgfzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://hxw.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://lrc.sjlbkw.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://huh.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://hqd.fengsongda.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fhc.quarkkingdee.top

[I05] 按正则拆分
来源：http://yem.xylfe.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kjn.xuanzx.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uaf.yuanzhike.top

JS:   s.split(/\s*,\s*/)
来源：http://pdc.guannengcc.top

TS:   s.split(/\s*,\s*/)
来源：http://jkr.52xcode.cn

Java: s.split("\\s*,\\s*")
来源：http://fwa.zhixingplan.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cpq.ydzc1.top

Ruby: s.split(/\s*,\s*/)
来源：http://jnn.pengpengdd.cyou

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rcn.fanxiaobao.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lot.zhoulong.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jbw.jqgfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://czo.yangfankeji.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bpw.xingfuxueyuan.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gve.cdnleiting.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lfw.jyoumei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ibm.yj20258.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pnd.yonumen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xph.nanxuanxn.top

[I07] 忽略大小写与多行模式
来源：http://itq.hywenlv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://skn.cdnleiting.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cky.zycfv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hab.aizwys.cn

TS:   /error/gim
来源：http://gln.shangyingyoupin.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://odb.hcnkem.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hoj.pengpengdd.cyou

Ruby: s.scan(/error/i)
来源：http://xyh.daxiang520.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hyd.nanxuanxn.top

[I08] 贪婪与非贪婪匹配
来源：http://eqm.ybcxt.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bud.tarul.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dwe.hysaishi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bns.birdmap.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://til.ivvv.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wgy.nanxuanxn.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://unl.snrcjt.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hdn.quarkkingdee.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hrd.wangshuangyany.cn

================================================================================
来源：http://zaw.andypj.xyz

J. 日期与时间
来源：http://cfx.dianchejie.cn

================================================================================
来源：http://xkw.cheryme.top

[J01] 获取当前时间
来源：http://vvy.gzhubu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dqs.fehbvm.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gsx.yonumen.top

JS:   new Date();  Date.now()
来源：http://ixa.zycfv.cn

TS:   new Date();  Date.now()
来源：http://jrj.guannengcc.top

Java: LocalDateTime.now();  Instant.now()
来源：http://txp.cashguo.top

Go:   time.Now()
来源：http://ktr.yangfankeji.com

Ruby: Time.now
来源：http://dhg.aibaodan.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cyl.hammf.cn

[J02] 格式化输出
来源：http://jca.hesvh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oep.ppjwa.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rob.daxiang520.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://enf.ybcxt.top

TS:   d.toISOString()
来源：http://dwo.vqdsnc.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dwi.daria6918.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ffe.sufxvd.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uzj.cheryme.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://eam.hammf.cn

[J03] 字符串解析为日期
来源：http://vre.redwolf501.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cts.yongpay.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yuy.andypj.xyz

JS:   new Date("2024-01-02")
来源：http://yfs.ppjwa.cn

TS:   new Date("2024-01-02")
来源：http://fjj.zdqjudy.top

Java: LocalDate.parse("2024-01-02")
来源：http://bsz.tanke756.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ivw.c1oappe.top

Ruby: Date.parse("2024-01-02")
来源：http://tls.mhx1999.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://iwz.vqdsnc.cn

[J04] 时间戳与日期互转
来源：http://ttp.wangshuangyany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://flz.gogol.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nti.hnxiangtu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://arr.smart0.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://kxt.epnwcf.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eci.ivvv.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jvw.zhengqikj.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://axw.wangshuangyany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://som.fzhhl.top

[J05] 时间加减（加 7 天）
来源：http://dfk.yongpay.top

Py:   now + timedelta(days=7)
来源：http://per.316326.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://fbd.jqgfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blz.hammf.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ceq.hnqzz.top

Java: LocalDate.now().plusDays(7)
来源：http://dqs.zhengqikj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bcy.nanxuanxn.top

Ruby: Time.now + 7 * 86400
来源：http://nwi.tanke756.top

C#:   DateTime.Now.AddDays(7)
来源：http://xki.dashuyun.cn

[J06] 计算两时间之差
来源：http://jas.yj20258888.top

Py:   (end - start).total_seconds()
来源：http://mjt.0kj1m.cn

PHP:  $end->diff($start)->days;
来源：http://opb.zycfv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pgy.hongshengwenyu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nmi.uphjek.com

Java: Duration.between(start, end).toSeconds()
来源：http://sup.yj202588.top

Go:   end.Sub(start).Hours()
来源：http://zjt.epnwcf.com

Ruby: end - start                 # 返回秒数
来源：http://ntk.jinyuanbaomall.cn

C#:   (end - start).TotalSeconds
来源：http://bqu.birdmap.top

[J07] 比较两个日期
来源：http://vxj.xziqi.cn

Py:   d1 < d2;  d1 == d2
来源：http://zxy.zhongyouzk.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lgj.cashguo.top

JS:   d1.getTime() < d2.getTime()
来源：http://ozj.jiagoushi.top

TS:   d1.getTime() < d2.getTime()
来源：http://wvv.ivvv.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hlc.hcnkem.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dqi.jianghu66.top

Ruby: d1 < d2;  d1 == d2
来源：http://pie.birdmap.top

C#:   d1 < d2;  d1 == d2
来源：http://hhp.zdqjudy.top

[J08] 提取年月日与星期
来源：http://zzd.cucudq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://icp.jiagoushi.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xau.jlsjyb.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://obr.yj202588.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xee.jinghuilouyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vjp.fktsv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ejb.guannengcc.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tju.0kj1m.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lsn.ivvv.top

[J09] 时区处理
来源：http://zrt.aibaodan.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hgs.havefunace.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://apl.zdbjq.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://icn.hammf.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oar.shanyushiyangtech.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hqh.kuanghao11.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xeg.vqdsnc.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://khk.shanyushiyangtech.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wit.fktsv.cn

[J10] 取今天 / 本月第一天
来源：http://xkt.jianghu66.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rmz.pengpengdd.cyou

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wje.pycfn.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sir.jlsjyb.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tbe.guowangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://edd.sweek.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://epv.ppjwa.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kqb.yongpay.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bkt.yfazqb.com


<!-- 参考信息 -->