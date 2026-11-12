代发 wailian999

Py:   isinstance(u, User)
来源：http://qli.yj202588.top

PHP:  $u instanceof User
来源：http://aga.redwolf501.top

JS:   u instanceof User
来源：http://fsd.nanxinkj.top

TS:   u instanceof User
来源：http://lvo.jianghu66.top

Java: u instanceof User
来源：http://twi.shanyushiyangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://voq.jiagoushi.top

Ruby: u.is_a?(User)
来源：http://hly.fktsv.cn

C#:   u is User
来源：http://dyq.shanyushiyangtech.top

[G14] 数据类 / record
来源：http://hgo.fzhhl.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rho.jinghuilouyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://xum.yangfankeji.com

JS:   // 无内置：普通类或对象字面量
来源：http://roq.zhijiandao.cn

TS:   type User = { name: string; age: number };
来源：http://let.aizwys.cn

Java: record User(String name, int age) {}
来源：http://ysf.feifeiyinyue.top

Go:   type User struct { Name string; Age int }
来源：http://zud.ctjpmb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zng.zhoulong.xyz

C#:   record User(string Name, int Age);
来源：http://acx.havefunace.top

[G15] 枚举
来源：http://yfc.jyoumei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://owb.zhijiandao.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uop.cqqwz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nug.316326.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yoi.zhengqikj.top

Java: enum Color { RED, GREEN }
来源：http://ylx.yangfankeji.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bxd.zhongyouzk.top

Ruby: Color = %i[red green].freeze
来源：http://eim.shanyushiyangtech.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pxu.cqqwz.cn

[G16] 对象转数组 / 字典
来源：http://drt.chenjidiqi.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jls.tanke756.top

PHP:  get_object_vars($obj);
来源：http://rvx.sxryk.cn

JS:   Object.entries(obj)
来源：http://xan.aibaodan.cn

TS:   Object.entries(obj)
来源：http://vuw.vehdjk.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kfm.yanxiufei.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cjp.yfazqb.com

Ruby: obj.instance_variables
来源：http://jqk.yuanzhike.top

C#:   // 用反射或 System.Text.Json
来源：http://xjm.tian-w.cn

================================================================================
来源：http://hdn.havefunace.top

H. 异常与错误处理
来源：http://dkk.yj20258.top

================================================================================
来源：http://try.fehbvm.com

[H01] try / catch 基础
来源：http://oex.ybcxt.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xcw.uphjek.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ink.zhengqikj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://imc.xingfuxueyuan.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tfb.zhixingplan.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vwy.redwolf501.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yrt.jiagoushi.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vru.dashuyun.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://amc.yvedp.cn

[H02] finally / ensure 收尾
来源：http://dnj.nanxinkj.top

Py:   try: f()⏎finally: cleanup()
来源：http://iac.hfpthk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ufd.aibaodan.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jty.cqqwz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://frj.aibaodan.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ryq.zhiwuduotai.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://low.snrcjt.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://znc.yuanzhike.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://nwr.snrcjt.cn

[H03] 主动抛出异常
来源：http://ijc.gotoacloud.top

Py:   raise ValueError("错误信息")
来源：http://pbd.tanke756.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bcl.iojbl.cn

JS:   throw new Error("错误信息");
来源：http://khw.guannengcc.top

TS:   throw new Error("错误信息");
来源：http://ecj.ydzc1.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nbt.yueranfly.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oyu.wangshuangyany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xyt.sufxvd.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gbo.zdbjq.cn

[H04] 自定义异常类型
来源：http://qbm.shangyingyoupin.top

Py:   class MyError(Exception): pass
来源：http://nic.birdmap.top

PHP:  class MyError extends RuntimeException {}
来源：http://dni.guannengcc.top

JS:   class MyError extends Error {}
来源：http://qft.quarkkingdee.top

TS:   class MyError extends Error {}
来源：http://sqp.aizwys.cn

Java: class MyException extends RuntimeException {}
来源：http://ptu.tanke756.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aqo.gzhubu.top

Ruby: class MyError < StandardError; end
来源：http://gad.gotoacloud.top

C#:   class MyException : Exception {}
来源：http://tzs.ydzc1.top

[H05] 捕获特定类型
来源：http://yzc.daria6918.cn

Py:   except ValueError as e:
来源：http://fct.316326.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hxi.tian-w.cn

JS:   if (e instanceof TypeError) {}
来源：http://daj.feifeiyinyue.top

TS:   if (e instanceof TypeError) {}
来源：http://tin.zhengqikj.top

Java: catch (IOException | SQLException e) {}
来源：http://dvb.ppjwa.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ewu.hnxiangtu.top

Ruby: rescue ArgumentError => e
来源：http://ocy.havefunace.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dvb.9152youxi.cn

[H06] 可选值 / 空值安全访问
来源：http://umb.dashuyun.cn

Py:   value = d.get("k") or default
来源：http://acl.epnwcf.com

PHP:  $v = $d["k"] ?? null;
来源：http://qti.zhengqikj.top

JS:   obj?.a?.b;  d ?? default
来源：http://lmx.xinyue.icu

TS:   obj?.a?.b;  d ?? default
来源：http://pvx.hfpthk.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lim.hongshengwenyu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jbj.daxiang520.top

Ruby: d&.dig(:a, :b)
来源：http://ijh.kuanghao11.cn

C#:   obj?.A?.B ?? default
来源：http://bay.yanxiufei.cn

[H07] 断言
来源：http://oio.hfpthk.cn

Py:   assert x > 0, "必须为正"
来源：http://ndz.kuanghao11.cn

PHP:  assert($x > 0);
来源：http://kgp.hywenlv.cn

JS:   console.assert(x > 0);
来源：http://hbu.316326.xyz

TS:   console.assert(x > 0);
来源：http://wvc.epnwcf.com

Java: assert x > 0 : "必须为正";
来源：http://vfs.quarkkingdee.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tan.quarkkingdee.top

Ruby: raise "必须为正" unless x > 0
来源：http://hnk.hesvh.cn

C#:   Debug.Assert(x > 0);
来源：http://gyj.uphjek.com

[H08] 获取错误信息与堆栈
来源：http://yxo.yongpay.top

Py:   str(e);  traceback.format_exc()
来源：http://mxn.cdnleiting.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://led.shangyingyoupin.top

JS:   e.message;  e.stack
来源：http://pal.nanxuanxn.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fsm.jqgufenzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://qrd.hcnkem.com

Go:   err.Error()
来源：http://fih.zhijiandao.cn

Ruby: e.message;  e.backtrace
来源：http://pls.vqdsnc.cn

C#:   e.Message;  e.StackTrace
来源：http://gqw.chenzaomai.com

[H09] 带错误码的异常
来源：http://ipe.yanxiufei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tyj.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hcx.jianghu66.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://idv.fktsv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wuj.fanxiaobao.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lxr.ehwqpu.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cfy.yongpay.top

Ruby: raise MyError.new("fail", 500)
来源：http://bcs.nanxuanxn.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kmg.yueranfly.top

[H10] 资源自动释放
来源：http://ogl.hysaishi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nfn.zhijiandao.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dvz.bjfxy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eid.havefunace.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mcw.svipenyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fxs.gogol.net.cn

Go:   defer f.Close()
来源：http://eto.guowangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wdz.guowangkeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mxb.bbcook.cn

================================================================================
来源：http://vyj.xylfe.cn

I. 正则表达式
来源：http://yfz.jyoumei.cn

================================================================================
来源：http://dvk.jianghu66.top

[I01] 判断是否匹配
来源：http://crl.fzhhl.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bkm.smart0.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://hpk.shanyushiyangkeji.top

JS:   /\d+/.test(s)
来源：http://yww.jinqigfzy.top

TS:   /\d+/.test(s)
来源：http://zzs.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ymt.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://crg.fehbvm.com

Ruby: s.match?(/\d+/)
来源：http://oyq.jqgfzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qdj.ctjpmb.com

[I02] 提取所有匹配
来源：http://fsd.nanxinkj.top

Py:   re.findall(r"\d+", s)
来源：http://eqf.xziqi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tzs.wangshuangyany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sjl.svipenyu.cn

TS:   s.match(/\d+/g)
来源：http://hnu.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ebf.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ppc.yj20258.top

Ruby: s.scan(/\d+/)
来源：http://fcz.cqqwz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://avp.hysaishi.cn

[I03] 提取捕获分组
来源：http://oxa.zdbjq.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xoh.jlsjyb.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://giy.vqdsnc.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://drw.cucudq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qli.hcnkem.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://aus.fehbvm.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bpx.sweek.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://smu.xylfe.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ass.shanyushiyangtech.top

[I04] 正则替换
来源：http://ufu.xziqi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://axo.hfpthk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dvf.jyoumei.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kzp.sysykeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://zln.yanxiufei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://heo.vehdjk.com

Go:   re.ReplaceAllString(s, "#")
来源：http://lgn.gaohongyu789.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mym.sjlbkw.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://upv.xziqi.cn

[I05] 按正则拆分
来源：http://noh.andypj.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://rss.sweek.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://iyu.yj202588.top

JS:   s.split(/\s*,\s*/)
来源：http://phu.bbcook.cn

TS:   s.split(/\s*,\s*/)
来源：http://igs.ybcxt.top

Java: s.split("\\s*,\\s*")
来源：http://nuh.nanxuanxn.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vri.shuidangran.top

Ruby: s.split(/\s*,\s*/)
来源：http://hrr.zhijiandao.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ifm.gogol.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://azm.tarul.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yzi.havefunace.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://itt.hongshengwenyu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kdg.yj202588.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://syh.jianghu66.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dxf.jinqigfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nxq.shzxlz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kmq.bjfxy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lhi.zhengqikj.top

[I07] 忽略大小写与多行模式
来源：http://epw.tian-w.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qxs.tian-w.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dok.jqgfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xom.vehdjk.com

TS:   /error/gim
来源：http://pwi.tanke756.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://utp.shzxlz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cxa.andypj.xyz

Ruby: s.scan(/error/i)
来源：http://xzs.hnqzz.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kbk.ydzc1.top

[I08] 贪婪与非贪婪匹配
来源：http://dpd.fzhhl.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tjo.gogol.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sab.pengpengdd.cyou

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cja.hongshengwenyu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yvt.shanyushiyangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://las.fktsv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wyu.yj202588.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kwd.yj202588.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ixd.wangdashe.top

================================================================================
来源：http://xnf.ppjwa.cn

J. 日期与时间
来源：http://uie.daria6918.cn

================================================================================
来源：http://kpg.hesvh.cn

[J01] 获取当前时间
来源：http://olg.bjfxy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://pip.hongshengwenyu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tjo.jinqigufen.top

JS:   new Date();  Date.now()
来源：http://lkt.bbcook.cn

TS:   new Date();  Date.now()
来源：http://cpk.daxiang520.top

Java: LocalDateTime.now();  Instant.now()
来源：http://plf.shzxlz.cn

Go:   time.Now()
来源：http://gjo.redwolf501.top

Ruby: Time.now
来源：http://mfr.sweek.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dmr.bjfxy.top

[J02] 格式化输出
来源：http://zmj.zhijiandao.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ect.ydjk.org.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kyd.bbcook.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dtt.shanyushiyangkeji.top

TS:   d.toISOString()
来源：http://wub.jianghu66.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pms.cqqwz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sdr.bjfxy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uyk.tarul.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ude.pycfn.com

[J03] 字符串解析为日期
来源：http://yit.xinyue.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fio.bbcook.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lhn.ybcxt.top

JS:   new Date("2024-01-02")
来源：http://stw.c1oappe.top

TS:   new Date("2024-01-02")
来源：http://aqp.uphjek.com

Java: LocalDate.parse("2024-01-02")
来源：http://rva.jyoumei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jlq.zhongyouzk.top

Ruby: Date.parse("2024-01-02")
来源：http://eut.tanke756.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gyr.vqdsnc.cn

[J04] 时间戳与日期互转
来源：http://aha.bjfxy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wyb.shzxlz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pii.pycfn.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zcg.quarkkingdee.top

TS:   Math.floor(Date.now() / 1000)
来源：http://rpu.sysykeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hzk.cucudq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gzf.hammf.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://aur.daxiang520.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://inz.svipenyu.cn

[J05] 时间加减（加 7 天）
来源：http://abm.jyoumei.cn

Py:   now + timedelta(days=7)
来源：http://dia.ctjpmb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ihl.zycfv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kjn.vehdjk.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wzj.cucudq.cn

Java: LocalDate.now().plusDays(7)
来源：http://dmq.svipenyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fcm.yfazqb.com

Ruby: Time.now + 7 * 86400
来源：http://nut.ydjk.org.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nmq.feifeiyinyue.top

[J06] 计算两时间之差
来源：http://gsg.yj202588.top

Py:   (end - start).total_seconds()
来源：http://zov.hfpthk.cn

PHP:  $end->diff($start)->days;
来源：http://vzp.zhaomingkeji.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qzs.xuetiantiany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ugx.havefunace.top

Java: Duration.between(start, end).toSeconds()
来源：http://fex.yuanzhike.top

Go:   end.Sub(start).Hours()
来源：http://hrc.shanyushiyangtech.top

Ruby: end - start                 # 返回秒数
来源：http://kaw.hesvh.cn

C#:   (end - start).TotalSeconds
来源：http://phn.jinqigufen.top

[J07] 比较两个日期
来源：http://wco.xuanzx.com

Py:   d1 < d2;  d1 == d2
来源：http://rqk.0kj1m.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xrc.tian-w.cn

JS:   d1.getTime() < d2.getTime()
来源：http://oey.shangyingyoupin.top

TS:   d1.getTime() < d2.getTime()
来源：http://fpv.tanke756.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zfv.c1oappe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jxh.cqqwz.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nmt.sweek.top

C#:   d1 < d2;  d1 == d2
来源：http://wkg.shangyingyoupin.top

[J08] 提取年月日与星期
来源：http://dvm.dashuyun.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qim.316326.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://htl.havefunace.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://npr.ydjk.org.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mjf.shzxlz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vfi.jianghu66.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yvq.zhoulong.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://upn.52xcode.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://etj.fengsongda.top

[J09] 时区处理
来源：http://zgk.yuanzhike.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fuk.xuanzx.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jgg.fktsv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hzf.ydjk.org.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vmh.shuidangran.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pjg.jqgufenzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jle.cheryme.top

Ruby: Time.now.getlocal("+08:00")
来源：http://whs.feifeiyinyue.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://afz.ywan-chungtsiang.top

[J10] 取今天 / 本月第一天
来源：http://geq.hfpthk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qrh.ehwqpu.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dgl.aizwys.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fkb.tanke756.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qzu.hcnkem.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nun.fehbvm.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hvc.xingfuxueyuan.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://arj.yueranfly.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vrg.shangyingyoupin.top

================================================================================
来源：http://lok.redwolf501.top

K. JSON 与序列化
来源：http://aak.haohaochexian.top

================================================================================
来源：http://dml.fzhhl.top

[K01] 对象转 JSON 字符串
来源：http://rgt.guowangkeji.top


<!-- 参考信息 -->