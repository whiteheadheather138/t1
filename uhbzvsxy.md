代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://tkv.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://lzi.zhongyouzk.top

C#:   public override string ToString() => Name;
来源：http://fcx.tian-w.cn

[G13] 判断对象类型
来源：http://los.yj20258888.top

Py:   isinstance(u, User)
来源：http://nwh.jqgufenzy.top

PHP:  $u instanceof User
来源：http://evq.gaohongyu789.top

JS:   u instanceof User
来源：http://egh.sufxvd.cn

TS:   u instanceof User
来源：http://dxn.birdmap.top

Java: u instanceof User
来源：http://eam.daria6918.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://woj.52xcode.cn

Ruby: u.is_a?(User)
来源：http://lkl.zhijiandao.cn

C#:   u is User
来源：http://dkj.redwolf501.top

[G14] 数据类 / record
来源：http://luw.hnqzz.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yco.zdbjq.cn

PHP:  // 用 readonly 属性模拟
来源：http://rru.ehwqpu.com

JS:   // 无内置：普通类或对象字面量
来源：http://kew.hnqzz.top

TS:   type User = { name: string; age: number };
来源：http://seb.kuanghao11.cn

Java: record User(String name, int age) {}
来源：http://jqh.iojbl.cn

Go:   type User struct { Name string; Age int }
来源：http://iou.guowangkeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gpm.tianlin.xyz

C#:   record User(string Name, int Age);
来源：http://aae.tanke756.top

[G15] 枚举
来源：http://aya.aizwys.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gjw.zhiwuduotai.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zrr.xingfuxueyuan.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lpf.cucudq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kib.yfazqb.com

Java: enum Color { RED, GREEN }
来源：http://ddc.tarul.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hfx.smart0.xyz

Ruby: Color = %i[red green].freeze
来源：http://nci.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://esm.chenjidiqi.icu

[G16] 对象转数组 / 字典
来源：http://rqg.xuetiantiany.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ths.xziqi.cn

PHP:  get_object_vars($obj);
来源：http://drz.hfpthk.cn

JS:   Object.entries(obj)
来源：http://fub.haohaochexian.top

TS:   Object.entries(obj)
来源：http://rev.vehdjk.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://svk.sjlbkw.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jbk.daria6918.cn

Ruby: obj.instance_variables
来源：http://tfu.yueranfly.top

C#:   // 用反射或 System.Text.Json
来源：http://mvx.gogol.net.cn

================================================================================
来源：http://jpa.zycfv.cn

H. 异常与错误处理
来源：http://vgy.iojbl.cn

================================================================================
来源：http://vsn.zhixingplan.top

[H01] try / catch 基础
来源：http://hhr.uphjek.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wik.ehwqpu.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gld.bjfxy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qcl.zhiwuduotai.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hdz.redwolf501.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eoo.xingfuxueyuan.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mct.guannengcc.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hth.haohaochexian.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ogw.sxryk.cn

[H02] finally / ensure 收尾
来源：http://brq.zhaomingkeji.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://dvc.fengsongda.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nnn.fehbvm.com

JS:   try { f(); } finally { cleanup(); }
来源：http://dik.hcnkem.com

TS:   try { f(); } finally { cleanup(); }
来源：http://buy.gogol.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dhn.sxryk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wjw.haohaochexian.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pvz.zhixingplan.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fzd.yongpay.top

[H03] 主动抛出异常
来源：http://zqs.sweek.top

Py:   raise ValueError("错误信息")
来源：http://obx.svipenyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tsx.sufxvd.cn

JS:   throw new Error("错误信息");
来源：http://zaq.birdmap.top

TS:   throw new Error("错误信息");
来源：http://wpi.sweek.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://vro.xylfe.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://epe.haohaochexian.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ljm.yfazqb.com

C#:   throw new ArgumentException("错误信息");
来源：http://thy.yj20258.top

[H04] 自定义异常类型
来源：http://gyd.xuetiantiany.cn

Py:   class MyError(Exception): pass
来源：http://bal.zycfv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fxz.jlsjyb.cn

JS:   class MyError extends Error {}
来源：http://liq.fehbvm.com

TS:   class MyError extends Error {}
来源：http://vfd.jiagoushi.top

Java: class MyException extends RuntimeException {}
来源：http://nnl.epnwcf.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zjj.cucudq.cn

Ruby: class MyError < StandardError; end
来源：http://qen.havefunace.top

C#:   class MyException : Exception {}
来源：http://agv.pycfn.com

[H05] 捕获特定类型
来源：http://dwr.wangdashe.top

Py:   except ValueError as e:
来源：http://bba.cucudq.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nko.nanxuanxn.top

JS:   if (e instanceof TypeError) {}
来源：http://ubt.zhengqikj.top

TS:   if (e instanceof TypeError) {}
来源：http://pdo.cucudq.cn

Java: catch (IOException | SQLException e) {}
来源：http://qpa.uphjek.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yuc.gzhubu.top

Ruby: rescue ArgumentError => e
来源：http://tha.ehwqpu.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dkg.shzxlz.cn

[H06] 可选值 / 空值安全访问
来源：http://ovv.yj20258.top

Py:   value = d.get("k") or default
来源：http://exp.hysaishi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ddw.0kj1m.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mwp.mhx1999.top

TS:   obj?.a?.b;  d ?? default
来源：http://xsj.zdqjudy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nza.hcnkem.com

Go:   if v, ok := m["k"]; ok { }
来源：http://cta.jinyuanbaomall.cn

Ruby: d&.dig(:a, :b)
来源：http://lxe.jqgfzy.top

C#:   obj?.A?.B ?? default
来源：http://yiw.dashuyun.cn

[H07] 断言
来源：http://ize.ppjwa.cn

Py:   assert x > 0, "必须为正"
来源：http://dgs.cashguo.top

PHP:  assert($x > 0);
来源：http://msn.ivvv.top

JS:   console.assert(x > 0);
来源：http://xkt.fehbvm.com

TS:   console.assert(x > 0);
来源：http://xxo.shangyingyoupin.top

Java: assert x > 0 : "必须为正";
来源：http://fbw.tanke756.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qlm.havefunace.top

Ruby: raise "必须为正" unless x > 0
来源：http://jie.hammf.cn

C#:   Debug.Assert(x > 0);
来源：http://zbr.shanyushiyangtech.top

[H08] 获取错误信息与堆栈
来源：http://npz.quarkkingdee.top

Py:   str(e);  traceback.format_exc()
来源：http://xgv.gogol.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gci.gaohongyu789.top

JS:   e.message;  e.stack
来源：http://xgb.ppjwa.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://iou.tarul.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pui.9152youxi.cn

Go:   err.Error()
来源：http://sxv.zhijiandao.cn

Ruby: e.message;  e.backtrace
来源：http://ung.zhongyouzk.top

C#:   e.Message;  e.StackTrace
来源：http://cvo.gogol.net.cn

[H09] 带错误码的异常
来源：http://udu.ydzc1.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hjc.andypj.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://rnh.dashuyun.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://utl.sweek.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://occ.zhoulong.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mry.guowangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ymm.guowangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://egj.xylfe.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wgo.xuanzx.com

[H10] 资源自动释放
来源：http://hug.hywenlv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qzw.nwbrower.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kog.shanyushiyangtech.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lsu.xylfe.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cdw.nanxinkj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eym.jyoumei.cn

Go:   defer f.Close()
来源：http://lgy.havefunace.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sxb.fzhhl.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yyo.ybcxt.top

================================================================================
来源：http://ibd.ehwqpu.com

I. 正则表达式
来源：http://pds.52xcode.cn

================================================================================
来源：http://waa.shanyushiyangtech.top

[I01] 判断是否匹配
来源：http://hwv.hammf.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yfi.cucudq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mpz.zhongyouzk.top

JS:   /\d+/.test(s)
来源：http://dbp.cheryme.top

TS:   /\d+/.test(s)
来源：http://oeu.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vve.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yxq.aizwys.cn

Ruby: s.match?(/\d+/)
来源：http://ibr.hnqzz.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qnr.pengpengdd.cyou

[I02] 提取所有匹配
来源：http://pff.fktsv.cn

Py:   re.findall(r"\d+", s)
来源：http://qmp.jianghu66.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ejo.yj202588.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ilz.aizwys.cn

TS:   s.match(/\d+/g)
来源：http://ogx.chenlongwang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://etw.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uir.ctjpmb.com

Ruby: s.scan(/\d+/)
来源：http://qhy.yvedp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mup.jiagoushi.top

[I03] 提取捕获分组
来源：http://rhq.bbcook.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dks.vqdsnc.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tnj.yuanzhike.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tld.sxryk.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hxr.vehdjk.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gvf.svipenyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rru.zhaomingkeji.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sih.hysaishi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://agm.xuetiantiany.cn

[I04] 正则替换
来源：http://qgl.sweek.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ema.cqqwz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://syt.sjlbkw.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ohd.fehbvm.com

TS:   s.replace(/\d+/g, "#")
来源：http://hhq.ivvv.top

Java: s.replaceAll("\\d+", "#")
来源：http://xrz.sufxvd.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nvj.wangshuangyany.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xgr.bjfxy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ymi.ivvv.top

[I05] 按正则拆分
来源：http://dil.yongpay.top

Py:   re.split(r"\s*,\s*", s)
来源：http://vvz.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://aww.andypj.xyz

JS:   s.split(/\s*,\s*/)
来源：http://xsn.epnwcf.com

TS:   s.split(/\s*,\s*/)
来源：http://jzs.wangshuangyany.cn

Java: s.split("\\s*,\\s*")
来源：http://cpg.gaohongyu789.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gvd.sufxvd.cn

Ruby: s.split(/\s*,\s*/)
来源：http://asg.ybcxt.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wgv.cdnleiting.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tbw.gogol.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bio.ydjk.org.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vop.hnqzz.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ucx.yj20258888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ucj.ywan-chungtsiang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sft.52xcode.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cku.hywenlv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tec.aibaodan.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dvl.zhoulong.xyz

[I07] 忽略大小写与多行模式
来源：http://cqo.yangfankeji.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hsg.sysykeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hmu.ivvv.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qsf.jyoumei.cn

TS:   /error/gim
来源：http://zpt.zhiwuduotai.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://aja.pycfn.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sny.52xcode.cn

Ruby: s.scan(/error/i)
来源：http://qsu.wangshuangyany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ghw.iojbl.cn

[I08] 贪婪与非贪婪匹配
来源：http://liz.hnxiangtu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vjq.yangfankeji.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kww.xylfe.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ngt.c1oappe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kbo.kuanghao11.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nvo.cashguo.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lsl.hnqzz.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jov.iojbl.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://itz.daria6918.cn

================================================================================
来源：http://ndw.uphjek.com

J. 日期与时间
来源：http://ddc.meibo888.top

================================================================================
来源：http://jva.fktsv.cn

[J01] 获取当前时间
来源：http://bvp.daxiang520.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gnv.jlsjyb.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nui.316326.xyz

JS:   new Date();  Date.now()
来源：http://lhg.pycfn.com

TS:   new Date();  Date.now()
来源：http://kle.shuidangran.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pkc.zdqjudy.top

Go:   time.Now()
来源：http://nmp.andypj.xyz

Ruby: Time.now
来源：http://iji.iojbl.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ehn.jinyuanbaomall.cn

[J02] 格式化输出
来源：http://krk.uphjek.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uvs.nwbrower.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gef.jqgufenzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fpo.hcnkem.com

TS:   d.toISOString()
来源：http://khg.jyoumei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://axp.jinghuilouyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lyb.ybcxt.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kdr.iojbl.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tax.mhx1999.top

[J03] 字符串解析为日期
来源：http://llp.uphjek.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://psg.nanxuanxn.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cdl.sjlbkw.cn

JS:   new Date("2024-01-02")
来源：http://mdt.gotoacloud.top

TS:   new Date("2024-01-02")
来源：http://yjt.wangshuangyany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bbi.redwolf501.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eak.xylfe.cn

Ruby: Date.parse("2024-01-02")
来源：http://rje.shuidangran.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://era.zhixingplan.top

[J04] 时间戳与日期互转
来源：http://dxe.xingfuxueyuan.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fmd.tianlin.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pxi.iojbl.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dyq.sxryk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fds.shuidangran.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vnr.uphjek.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wgi.feifeiyinyue.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fbw.sysykeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://esd.hywenlv.cn

[J05] 时间加减（加 7 天）
来源：http://xgg.mhx1999.top

Py:   now + timedelta(days=7)
来源：http://dvz.hcnkem.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ysb.iojbl.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hqk.yuanzhike.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jnh.fktsv.cn

Java: LocalDate.now().plusDays(7)
来源：http://aon.chenjidiqi.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ztd.yj20258.top

Ruby: Time.now + 7 * 86400
来源：http://sdh.nwbrower.top

C#:   DateTime.Now.AddDays(7)
来源：http://ywl.tian-w.cn

[J06] 计算两时间之差
来源：http://zea.sxryk.cn

Py:   (end - start).total_seconds()
来源：http://emh.jianghu66.top

PHP:  $end->diff($start)->days;
来源：http://png.ppjwa.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://irt.chenlongwang.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wfh.yj20258888.top

Java: Duration.between(start, end).toSeconds()
来源：http://gjg.ivvv.top

Go:   end.Sub(start).Hours()
来源：http://ymu.sufxvd.cn

Ruby: end - start                 # 返回秒数
来源：http://tdd.ppjwa.cn

C#:   (end - start).TotalSeconds
来源：http://xcb.xziqi.cn

[J07] 比较两个日期
来源：http://wpt.gaohongyu789.top

Py:   d1 < d2;  d1 == d2
来源：http://yak.dianchejie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ebt.jyoumei.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bjt.yfazqb.com

TS:   d1.getTime() < d2.getTime()
来源：http://pmb.hammf.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lds.jinqigfzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kox.9152youxi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zlj.jlsjyb.cn

C#:   d1 < d2;  d1 == d2
来源：http://xvy.meibo888.top

[J08] 提取年月日与星期
来源：http://coq.ehwqpu.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gph.jinyuanbaomall.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://add.zdbjq.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pbd.gzhubu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bfv.fengsongda.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yne.uphjek.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qxv.pycfn.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gyx.guowangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sxv.jlsjyb.cn

[J09] 时区处理
来源：http://chk.epnwcf.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uyb.yanxiufei.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ufz.bjfxy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://prl.sjlbkw.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iod.zhixingplan.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xju.shuidangran.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wie.yvedp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uvj.guannengcc.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fvx.cucudq.cn

[J10] 取今天 / 本月第一天
来源：http://smz.ydzc1.top

Py:   date.today();  date.today().replace(day=1)
来源：http://nki.gogol.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rzf.chenjidiqi.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bdu.ivvv.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tdh.hongshengwenyu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dav.zhiwuduotai.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hsr.zhiwuduotai.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://woo.yonumen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wfl.uphjek.com


<!-- 参考信息 -->