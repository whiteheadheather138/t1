代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://rln.ywan-chungtsiang.top

Ruby: def to_s; @name; end
来源：http://fjj.feifeiyinyue.top

C#:   public override string ToString() => Name;
来源：http://snu.nanxinkj.top

[G13] 判断对象类型
来源：http://lie.gotoacloud.top

Py:   isinstance(u, User)
来源：http://utz.ybcxt.top

PHP:  $u instanceof User
来源：http://axt.dashuyun.cn

JS:   u instanceof User
来源：http://vfi.epnwcf.com

TS:   u instanceof User
来源：http://gic.yanxiufei.cn

Java: u instanceof User
来源：http://vsq.jiagoushi.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://drl.hnqzz.top

Ruby: u.is_a?(User)
来源：http://egq.tianlin.xyz

C#:   u is User
来源：http://jmh.xuanzx.com

[G14] 数据类 / record
来源：http://ivw.yonumen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mlh.hfpthk.cn

PHP:  // 用 readonly 属性模拟
来源：http://xpr.hnxiangtu.top

JS:   // 无内置：普通类或对象字面量
来源：http://qpl.zhongyouzk.top

TS:   type User = { name: string; age: number };
来源：http://boo.xylfe.cn

Java: record User(String name, int age) {}
来源：http://krz.shuidangran.top

Go:   type User struct { Name string; Age int }
来源：http://krw.cqqwz.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mpc.zhiwuduotai.top

C#:   record User(string Name, int Age);
来源：http://cxg.smart0.xyz

[G15] 枚举
来源：http://blh.gotoacloud.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pju.shangyingyoupin.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ayh.gotoacloud.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eas.yonumen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ora.hysaishi.cn

Java: enum Color { RED, GREEN }
来源：http://vec.zhiwuduotai.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nbh.fktsv.cn

Ruby: Color = %i[red green].freeze
来源：http://lei.ywan-chungtsiang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ddj.yanxiufei.cn

[G16] 对象转数组 / 字典
来源：http://iyk.fktsv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xoy.fzhhl.top

PHP:  get_object_vars($obj);
来源：http://zfr.nwbrower.top

JS:   Object.entries(obj)
来源：http://kpn.ybcxt.top

TS:   Object.entries(obj)
来源：http://yki.hesvh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://djr.chenzaomai.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://zcq.zhoulong.xyz

Ruby: obj.instance_variables
来源：http://toa.wangdashe.top

C#:   // 用反射或 System.Text.Json
来源：http://cwt.redwolf501.top

================================================================================
来源：http://aey.yanxiufei.cn

H. 异常与错误处理
来源：http://ter.hesvh.cn

================================================================================
来源：http://uot.chenjidiqi.icu

[H01] try / catch 基础
来源：http://uhk.snrcjt.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lmr.ctjpmb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dyq.gotoacloud.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xik.cashguo.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fag.0kj1m.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ots.havefunace.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hom.chenjidiqi.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kvg.yuanzhike.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bon.nanxuanxn.top

[H02] finally / ensure 收尾
来源：http://wvt.jlsjyb.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dxb.gogol.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lmp.meibo888.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xkk.ivvv.top

TS:   try { f(); } finally { cleanup(); }
来源：http://siz.ppjwa.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ljp.tianlin.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://upr.yongpay.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fev.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://uub.svipenyu.cn

[H03] 主动抛出异常
来源：http://wai.chenlongwang.top

Py:   raise ValueError("错误信息")
来源：http://svc.fengsongda.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nmc.guowangkeji.top

JS:   throw new Error("错误信息");
来源：http://uxi.fanxiaobao.xyz

TS:   throw new Error("错误信息");
来源：http://jus.sweek.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mst.xingfuxueyuan.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://duj.xziqi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kfz.c1oappe.top

C#:   throw new ArgumentException("错误信息");
来源：http://xul.bbcook.cn

[H04] 自定义异常类型
来源：http://ivv.nanxinkj.top

Py:   class MyError(Exception): pass
来源：http://uth.yongpay.top

PHP:  class MyError extends RuntimeException {}
来源：http://rko.ydjk.org.cn

JS:   class MyError extends Error {}
来源：http://yrw.yonumen.top

TS:   class MyError extends Error {}
来源：http://jwa.chenlongwang.top

Java: class MyException extends RuntimeException {}
来源：http://kok.nwbrower.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xwn.yj20258.top

Ruby: class MyError < StandardError; end
来源：http://jdc.yj20258888.top

C#:   class MyException : Exception {}
来源：http://tlb.sxryk.cn

[H05] 捕获特定类型
来源：http://deh.haohaochexian.top

Py:   except ValueError as e:
来源：http://qsa.tarul.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gue.ydzc1.top

JS:   if (e instanceof TypeError) {}
来源：http://qmb.sysykeji.top

TS:   if (e instanceof TypeError) {}
来源：http://bvp.zhixingplan.top

Java: catch (IOException | SQLException e) {}
来源：http://vxi.gzhubu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://trs.iojbl.cn

Ruby: rescue ArgumentError => e
来源：http://kts.zhongyouzk.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pwx.tarul.cn

[H06] 可选值 / 空值安全访问
来源：http://gdq.nanxuanxn.top

Py:   value = d.get("k") or default
来源：http://yiz.zhoulong.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://zuo.jianghu66.top

JS:   obj?.a?.b;  d ?? default
来源：http://ran.ivvv.top

TS:   obj?.a?.b;  d ?? default
来源：http://xwq.jqgfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yqc.yanxiufei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ngv.shanyushiyangtech.top

Ruby: d&.dig(:a, :b)
来源：http://bwf.cqqwz.cn

C#:   obj?.A?.B ?? default
来源：http://cwy.iojbl.cn

[H07] 断言
来源：http://vqo.ywan-chungtsiang.top

Py:   assert x > 0, "必须为正"
来源：http://tpg.shzxlz.cn

PHP:  assert($x > 0);
来源：http://gbq.cashguo.top

JS:   console.assert(x > 0);
来源：http://mki.quarkkingdee.top

TS:   console.assert(x > 0);
来源：http://jwb.aizwys.cn

Java: assert x > 0 : "必须为正";
来源：http://hrq.hnxiangtu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gof.svipenyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://axw.kuanghao11.cn

C#:   Debug.Assert(x > 0);
来源：http://nqo.wangshuangyany.cn

[H08] 获取错误信息与堆栈
来源：http://kxe.hcnkem.com

Py:   str(e);  traceback.format_exc()
来源：http://mkr.yuanzhike.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ste.kuanghao11.cn

JS:   e.message;  e.stack
来源：http://jei.wangdashe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ipk.yueranfly.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zyx.zhaomingkeji.xyz

Go:   err.Error()
来源：http://xov.yanxiufei.cn

Ruby: e.message;  e.backtrace
来源：http://prd.ydjk.org.cn

C#:   e.Message;  e.StackTrace
来源：http://wya.xziqi.cn

[H09] 带错误码的异常
来源：http://ztu.aibaodan.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vue.zhongyouzk.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ybm.yj20258.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xhh.ywan-chungtsiang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fjx.zdqjudy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://diw.ppjwa.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wxb.birdmap.top

Ruby: raise MyError.new("fail", 500)
来源：http://zie.fanxiaobao.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://evk.ydzc1.top

[H10] 资源自动释放
来源：http://igf.tanke756.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lqo.dashuyun.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://snv.hnqzz.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mjz.yangfankeji.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xjs.nanxinkj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://feq.hesvh.cn

Go:   defer f.Close()
来源：http://hnt.cucudq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ips.ydzc1.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lxw.zhoulong.xyz

================================================================================
来源：http://evt.birdmap.top

I. 正则表达式
来源：http://ntk.guowangkeji.top

================================================================================
来源：http://zym.zycfv.cn

[I01] 判断是否匹配
来源：http://tce.andypj.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nng.smart0.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://acg.zhoulong.xyz

JS:   /\d+/.test(s)
来源：http://pzv.jinyuanbaomall.cn

TS:   /\d+/.test(s)
来源：http://ybd.shuidangran.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ufr.yj202588.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uwi.yanxiufei.cn

Ruby: s.match?(/\d+/)
来源：http://fhy.cucudq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mfp.zdbjq.cn

[I02] 提取所有匹配
来源：http://lud.guannengcc.top

Py:   re.findall(r"\d+", s)
来源：http://gjo.nanxuanxn.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qhe.shzxlz.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pri.daria6918.cn

TS:   s.match(/\d+/g)
来源：http://jde.9152youxi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wvk.yueranfly.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hir.jiagoushi.top

Ruby: s.scan(/\d+/)
来源：http://mip.0kj1m.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nla.316326.xyz

[I03] 提取捕获分组
来源：http://ohv.sufxvd.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cwv.bbcook.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cuw.yj20258.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xsk.ywan-chungtsiang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nwn.aibaodan.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jbm.xingfuxueyuan.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ely.hnqzz.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ush.sysykeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lue.yuxming.cn

[I04] 正则替换
来源：http://esx.zhaomingkeji.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://onx.zhijiandao.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ylo.havefunace.top

JS:   s.replace(/\d+/g, "#")
来源：http://ukj.jyoumei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://boz.fehbvm.com

Java: s.replaceAll("\\d+", "#")
来源：http://pcx.vehdjk.com

Go:   re.ReplaceAllString(s, "#")
来源：http://vcq.dianchejie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jrp.gogol.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://klp.gogol.net.cn

[I05] 按正则拆分
来源：http://mnc.hnqzz.top

Py:   re.split(r"\s*,\s*", s)
来源：http://sce.feifeiyinyue.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kzk.cucudq.cn

JS:   s.split(/\s*,\s*/)
来源：http://hkg.yuanzhike.top

TS:   s.split(/\s*,\s*/)
来源：http://gvr.zhijiandao.cn

Java: s.split("\\s*,\\s*")
来源：http://vyl.xuetiantiany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ptx.cashguo.top

Ruby: s.split(/\s*,\s*/)
来源：http://odn.aizwys.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://keh.pycfn.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aar.dashuyun.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://for.birdmap.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iqu.pycfn.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dlt.feifeiyinyue.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uta.ppjwa.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ecc.jlsjyb.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vip.yanxiufei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dvw.dashuyun.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://coq.kuanghao11.cn

[I07] 忽略大小写与多行模式
来源：http://grt.xylfe.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ygo.ydjk.org.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://unh.meibo888.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jmx.fktsv.cn

TS:   /error/gim
来源：http://wqg.ybcxt.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://act.fehbvm.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lxw.yuanzhike.top

Ruby: s.scan(/error/i)
来源：http://qiz.yongpay.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zjz.dianchejie.cn

[I08] 贪婪与非贪婪匹配
来源：http://vgl.yangfankeji.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://snx.zdbjq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://goh.ybcxt.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hky.jiagoushi.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://azj.dashuyun.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vnr.yangfankeji.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://clo.cdnleiting.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xuq.tian-w.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bxy.fanxiaobao.xyz

================================================================================
来源：http://iyo.hnxiangtu.top

J. 日期与时间
来源：http://ljy.chenzaomai.com

================================================================================
来源：http://gtm.hnxiangtu.top

[J01] 获取当前时间
来源：http://jga.yongpay.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hxa.gotoacloud.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://svx.epnwcf.com

JS:   new Date();  Date.now()
来源：http://cnt.yuxming.cn

TS:   new Date();  Date.now()
来源：http://prf.chenlongwang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gqj.meibo888.top

Go:   time.Now()
来源：http://xxd.jinghuilouyu.cn

Ruby: Time.now
来源：http://olr.redwolf501.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://emn.quarkkingdee.top

[J02] 格式化输出
来源：http://tbg.jlsjyb.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tzp.ydzc1.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fvj.epnwcf.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://spd.fehbvm.com

TS:   d.toISOString()
来源：http://ned.fehbvm.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vku.hesvh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nzd.shanyushiyangtech.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://svv.0kj1m.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oqm.birdmap.top

[J03] 字符串解析为日期
来源：http://ihp.fengsongda.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://twk.jlsjyb.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ijo.fengsongda.top

JS:   new Date("2024-01-02")
来源：http://yto.ybcxt.top

TS:   new Date("2024-01-02")
来源：http://yvh.gaohongyu789.top

Java: LocalDate.parse("2024-01-02")
来源：http://goj.haohaochexian.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wvx.fehbvm.com

Ruby: Date.parse("2024-01-02")
来源：http://lkf.haohaochexian.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://emv.jqgufenzy.top

[J04] 时间戳与日期互转
来源：http://bml.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://idu.shzxlz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gok.sysykeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yvd.zhongyouzk.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qpf.ydjk.org.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://urf.zhiwuduotai.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ovp.yongpay.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://amp.jinyuanbaomall.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kxv.svipenyu.cn

[J05] 时间加减（加 7 天）
来源：http://akq.yvedp.cn

Py:   now + timedelta(days=7)
来源：http://iof.hesvh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ttl.nanxinkj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pmx.epnwcf.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cpq.zdbjq.cn

Java: LocalDate.now().plusDays(7)
来源：http://hfg.jianghu66.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yni.zhongyouzk.top

Ruby: Time.now + 7 * 86400
来源：http://lyw.hesvh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dfl.tian-w.cn

[J06] 计算两时间之差
来源：http://afy.chenzaomai.com

Py:   (end - start).total_seconds()
来源：http://jxr.zycfv.cn

PHP:  $end->diff($start)->days;
来源：http://sef.guannengcc.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://syg.xuetiantiany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ytc.shzxlz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://whk.hfpthk.cn

Go:   end.Sub(start).Hours()
来源：http://hde.shzxlz.cn

Ruby: end - start                 # 返回秒数
来源：http://soh.feifeiyinyue.top

C#:   (end - start).TotalSeconds
来源：http://mzb.bbcook.cn

[J07] 比较两个日期
来源：http://lvn.ydjk.org.cn

Py:   d1 < d2;  d1 == d2
来源：http://lnr.ivvv.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ghu.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://jrl.xziqi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dmx.redwolf501.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jub.svipenyu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://esb.bjfxy.top

Ruby: d1 < d2;  d1 == d2
来源：http://tua.zhaomingkeji.xyz

C#:   d1 < d2;  d1 == d2
来源：http://hjj.epnwcf.com

[J08] 提取年月日与星期
来源：http://apv.xinyue.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kwi.ppjwa.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hib.yj202588.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uin.shuidangran.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dmx.tian-w.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zar.hcnkem.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rtm.feifeiyinyue.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sef.zhaomingkeji.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nal.shanyushiyangtech.top

[J09] 时区处理
来源：http://xbe.gaohongyu789.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://liv.wangdashe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://avk.tianlin.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kiu.jyoumei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hcg.ydjk.org.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gqq.daria6918.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sqw.meibo888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vwo.cheryme.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vpk.fehbvm.com

[J10] 取今天 / 本月第一天
来源：http://nwr.nwbrower.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vho.jinghuilouyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pne.shuidangran.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nmx.xuetiantiany.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yby.yfazqb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://giy.tanke756.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://unn.sysykeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://osu.yj20258888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qod.jinghuilouyu.cn


<!-- 参考信息 -->