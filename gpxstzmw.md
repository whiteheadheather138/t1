代发 wailian999

JS:   get name() { return this._name; }
来源：http://yku.yangfankeji.com

TS:   get name(): string { return this._name; }
来源：http://udk.chenjidiqi.icu

Java: public String getName() { return name; }
来源：http://ant.yj202588.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ujx.jqgufenzy.top

Ruby: attr_accessor :name
来源：http://wwg.fktsv.cn

C#:   public string Name { get; set; }
来源：http://wwk.guannengcc.top

[G12] 对象转字符串
来源：http://tum.zhixingplan.top

Py:   def __str__(self): return self.name
来源：http://yto.shanyushiyangkeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zxn.guowangkeji.top

JS:   toString() { return this.name; }
来源：http://iwe.feifeiyinyue.top

TS:   toString(): string { return this.name; }
来源：http://mmm.chenlongwang.top

Java: @Override public String toString() { return name; }
来源：http://wwk.hammf.cn

Go:   func (u User) String() string { return u.Name }
来源：http://eyt.fktsv.cn

Ruby: def to_s; @name; end
来源：http://xhd.hesvh.cn

C#:   public override string ToString() => Name;
来源：http://lkk.fzhhl.top

[G13] 判断对象类型
来源：http://bvf.shanyushiyangkeji.top

Py:   isinstance(u, User)
来源：http://fwp.fzhhl.top

PHP:  $u instanceof User
来源：http://ldy.yanxiufei.cn

JS:   u instanceof User
来源：http://qig.uphjek.com

TS:   u instanceof User
来源：http://vsa.yanxiufei.cn

Java: u instanceof User
来源：http://ggv.gzhubu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wrq.nanxuanxn.top

Ruby: u.is_a?(User)
来源：http://uyo.jqgfzy.top

C#:   u is User
来源：http://fuq.ctjpmb.com

[G14] 数据类 / record
来源：http://ajb.jinyuanbaomall.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://npi.yj20258888.top

PHP:  // 用 readonly 属性模拟
来源：http://gaq.hammf.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bde.quarkkingdee.top

TS:   type User = { name: string; age: number };
来源：http://zfp.jlsjyb.cn

Java: record User(String name, int age) {}
来源：http://ygh.yj20258888.top

Go:   type User struct { Name string; Age int }
来源：http://jhk.hcnkem.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cbi.cheryme.top

C#:   record User(string Name, int Age);
来源：http://fka.xziqi.cn

[G15] 枚举
来源：http://hxp.cqqwz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bud.smart0.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://vrh.0kj1m.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ihn.guowangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://urc.ivvv.top

Java: enum Color { RED, GREEN }
来源：http://fwf.aizwys.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rke.jinghuilouyu.cn

Ruby: Color = %i[red green].freeze
来源：http://blu.uphjek.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lvn.xziqi.cn

[G16] 对象转数组 / 字典
来源：http://jxy.zhaomingkeji.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yqn.xylfe.cn

PHP:  get_object_vars($obj);
来源：http://kcq.aizwys.cn

JS:   Object.entries(obj)
来源：http://pui.jinqigufen.top

TS:   Object.entries(obj)
来源：http://svq.yj20258888.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bry.bjfxy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://pps.ybcxt.top

Ruby: obj.instance_variables
来源：http://dae.gzhubu.top

C#:   // 用反射或 System.Text.Json
来源：http://xqa.haohaochexian.top

================================================================================
来源：http://lot.cdnleiting.top

H. 异常与错误处理
来源：http://ish.jqgfzy.top

================================================================================
来源：http://wtm.yj202588.top

[H01] try / catch 基础
来源：http://ioj.gotoacloud.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rze.bjfxy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mwc.dashuyun.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nhs.svipenyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bwb.hcnkem.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wyx.zdbjq.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vpa.zhoulong.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iom.nwbrower.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mlh.iojbl.cn

[H02] finally / ensure 收尾
来源：http://kxy.hcnkem.com

Py:   try: f()⏎finally: cleanup()
来源：http://vnb.cashguo.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://wkj.shanyushiyangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://mdo.zhiwuduotai.top

TS:   try { f(); } finally { cleanup(); }
来源：http://egv.hfpthk.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ozh.sjlbkw.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hta.cashguo.top

Ruby: begin; f; ensure; cleanup; end
来源：http://cmm.xinyue.icu

C#:   try { F(); } finally { Cleanup(); }
来源：http://shc.pycfn.com

[H03] 主动抛出异常
来源：http://ikp.sxryk.cn

Py:   raise ValueError("错误信息")
来源：http://inu.jlsjyb.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://smd.birdmap.top

JS:   throw new Error("错误信息");
来源：http://moz.chenzaomai.com

TS:   throw new Error("错误信息");
来源：http://txk.fzhhl.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wpy.hnqzz.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rzu.fzhhl.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fgb.jinqigfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://nyj.bjfxy.top

[H04] 自定义异常类型
来源：http://kix.aibaodan.cn

Py:   class MyError(Exception): pass
来源：http://awq.xylfe.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ykp.ppjwa.cn

JS:   class MyError extends Error {}
来源：http://dbu.yuxming.cn

TS:   class MyError extends Error {}
来源：http://fui.tianlin.xyz

Java: class MyException extends RuntimeException {}
来源：http://gox.dashuyun.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://szi.redwolf501.top

Ruby: class MyError < StandardError; end
来源：http://vem.sysykeji.top

C#:   class MyException : Exception {}
来源：http://rgg.xingfuxueyuan.xyz

[H05] 捕获特定类型
来源：http://ocy.316326.xyz

Py:   except ValueError as e:
来源：http://iub.hnxiangtu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vux.haohaochexian.top

JS:   if (e instanceof TypeError) {}
来源：http://hvr.zhaomingkeji.xyz

TS:   if (e instanceof TypeError) {}
来源：http://fwp.fehbvm.com

Java: catch (IOException | SQLException e) {}
来源：http://odb.yueranfly.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://adq.mhx1999.top

Ruby: rescue ArgumentError => e
来源：http://nvf.jyoumei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vwg.shzxlz.cn

[H06] 可选值 / 空值安全访问
来源：http://vir.c1oappe.top

Py:   value = d.get("k") or default
来源：http://vzj.gzhubu.top

PHP:  $v = $d["k"] ?? null;
来源：http://crj.jqgfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://ksf.sweek.top

TS:   obj?.a?.b;  d ?? default
来源：http://mir.birdmap.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gzs.vehdjk.com

Go:   if v, ok := m["k"]; ok { }
来源：http://pci.nanxuanxn.top

Ruby: d&.dig(:a, :b)
来源：http://shi.feifeiyinyue.top

C#:   obj?.A?.B ?? default
来源：http://ual.jyoumei.cn

[H07] 断言
来源：http://ogg.yuxming.cn

Py:   assert x > 0, "必须为正"
来源：http://ird.andypj.xyz

PHP:  assert($x > 0);
来源：http://thf.sufxvd.cn

JS:   console.assert(x > 0);
来源：http://gxy.c1oappe.top

TS:   console.assert(x > 0);
来源：http://qdn.sysykeji.top

Java: assert x > 0 : "必须为正";
来源：http://ueg.shuidangran.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dcd.svipenyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gpw.ivvv.top

C#:   Debug.Assert(x > 0);
来源：http://jnp.shuidangran.top

[H08] 获取错误信息与堆栈
来源：http://zbb.zdbjq.cn

Py:   str(e);  traceback.format_exc()
来源：http://dde.ywan-chungtsiang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gdd.iojbl.cn

JS:   e.message;  e.stack
来源：http://vqp.zdbjq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xdu.yuanzhike.top

Java: e.getMessage();  e.printStackTrace()
来源：http://oli.yfazqb.com

Go:   err.Error()
来源：http://fqg.c1oappe.top

Ruby: e.message;  e.backtrace
来源：http://zae.chenzaomai.com

C#:   e.Message;  e.StackTrace
来源：http://rhq.hywenlv.cn

[H09] 带错误码的异常
来源：http://rdz.feifeiyinyue.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xcn.xingfuxueyuan.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://vou.sufxvd.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ftj.snrcjt.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sba.zhengqikj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://krn.jyoumei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lsh.vqdsnc.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zfg.yonumen.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zmw.yfazqb.com

[H10] 资源自动释放
来源：http://ysw.zdbjq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qph.shanyushiyangtech.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qza.chenzaomai.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ibu.hammf.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wqw.cdnleiting.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pex.sweek.top

Go:   defer f.Close()
来源：http://scg.ydzc1.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tmg.hywenlv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lam.xziqi.cn

================================================================================
来源：http://avv.ydzc1.top

I. 正则表达式
来源：http://odu.tian-w.cn

================================================================================
来源：http://pnp.52xcode.cn

[I01] 判断是否匹配
来源：http://cok.hammf.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://aku.fanxiaobao.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://neq.xinyue.icu

JS:   /\d+/.test(s)
来源：http://wbg.shzxlz.cn

TS:   /\d+/.test(s)
来源：http://xlv.tarul.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rbl.fzhhl.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pup.bbcook.cn

Ruby: s.match?(/\d+/)
来源：http://meu.nanxinkj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sdp.jinyuanbaomall.cn

[I02] 提取所有匹配
来源：http://qzj.andypj.xyz

Py:   re.findall(r"\d+", s)
来源：http://wgl.havefunace.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qff.fehbvm.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ady.epnwcf.com

TS:   s.match(/\d+/g)
来源：http://ofh.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kzm.yuxming.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vmm.c1oappe.top

Ruby: s.scan(/\d+/)
来源：http://uhi.zhengqikj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uvw.chenjidiqi.icu

[I03] 提取捕获分组
来源：http://mcs.9152youxi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qlh.chenjidiqi.icu

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kaa.fanxiaobao.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yjl.fktsv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pld.xylfe.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://knq.sysykeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ikn.tianlin.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gap.yongpay.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bna.jiagoushi.top

[I04] 正则替换
来源：http://gyl.ybcxt.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nra.nwbrower.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bke.zhengqikj.top

JS:   s.replace(/\d+/g, "#")
来源：http://fbv.chenjidiqi.icu

TS:   s.replace(/\d+/g, "#")
来源：http://qej.cdnleiting.top

Java: s.replaceAll("\\d+", "#")
来源：http://fbs.uphjek.com

Go:   re.ReplaceAllString(s, "#")
来源：http://lql.mhx1999.top

Ruby: s.gsub(/\d+/, "#")
来源：http://iio.jinqigufen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gae.hesvh.cn

[I05] 按正则拆分
来源：http://wdr.zhoulong.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://tjv.fanxiaobao.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tze.cheryme.top

JS:   s.split(/\s*,\s*/)
来源：http://foa.sweek.top

TS:   s.split(/\s*,\s*/)
来源：http://cgk.epnwcf.com

Java: s.split("\\s*,\\s*")
来源：http://qau.chenlongwang.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hoa.feifeiyinyue.top

Ruby: s.split(/\s*,\s*/)
来源：http://lmj.dashuyun.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://khq.shzxlz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lbc.hysaishi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bhz.wangdashe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kjw.sufxvd.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qig.c1oappe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bkd.sweek.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://afl.guannengcc.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tmj.aibaodan.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rft.sxryk.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jdf.tianlin.xyz

[I07] 忽略大小写与多行模式
来源：http://feo.tanke756.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rjf.daxiang520.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://brb.hongshengwenyu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rgn.52xcode.cn

TS:   /error/gim
来源：http://knq.cqqwz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rym.zhiwuduotai.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mcv.hesvh.cn

Ruby: s.scan(/error/i)
来源：http://vxj.zdqjudy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fvx.fktsv.cn

[I08] 贪婪与非贪婪匹配
来源：http://jsf.quarkkingdee.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ojy.yongpay.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kms.yuanzhike.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://shc.jinqigufen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gal.zhengqikj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ctx.jqgfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aqc.iojbl.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ipl.tian-w.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ruq.yj202588.top

================================================================================
来源：http://bzj.mhx1999.top

J. 日期与时间
来源：http://uvo.gzhubu.top

================================================================================
来源：http://pcg.316326.xyz

[J01] 获取当前时间
来源：http://fua.quarkkingdee.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mzm.hnqzz.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://owu.xingfuxueyuan.xyz

JS:   new Date();  Date.now()
来源：http://mlk.ywan-chungtsiang.top

TS:   new Date();  Date.now()
来源：http://pwu.guowangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://zgz.sjlbkw.cn

Go:   time.Now()
来源：http://mni.yfazqb.com

Ruby: Time.now
来源：http://edm.c1oappe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jov.dashuyun.cn

[J02] 格式化输出
来源：http://wik.xziqi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pzq.cqqwz.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wsl.smart0.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mtb.yj20258888.top

TS:   d.toISOString()
来源：http://niu.dianchejie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nwr.gaohongyu789.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gsc.nanxinkj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tgr.snrcjt.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vub.hywenlv.cn

[J03] 字符串解析为日期
来源：http://zrn.hnqzz.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gpz.redwolf501.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jlc.jqgfzy.top

JS:   new Date("2024-01-02")
来源：http://rfw.cashguo.top

TS:   new Date("2024-01-02")
来源：http://urs.zhaomingkeji.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://abc.jqgfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iqt.cqqwz.cn

Ruby: Date.parse("2024-01-02")
来源：http://qkb.yongpay.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://del.shuidangran.top

[J04] 时间戳与日期互转
来源：http://hjn.shanyushiyangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ubn.52xcode.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tni.meibo888.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gbo.sxryk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://akb.yuanzhike.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rfh.316326.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wzp.gotoacloud.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fqg.iojbl.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://osu.shangyingyoupin.top

[J05] 时间加减（加 7 天）
来源：http://cox.dashuyun.cn

Py:   now + timedelta(days=7)
来源：http://uqc.sufxvd.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qsf.zhijiandao.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yzq.sysykeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ybc.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://onq.yj202588.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rvm.quarkkingdee.top

Ruby: Time.now + 7 * 86400
来源：http://uus.pengpengdd.cyou

C#:   DateTime.Now.AddDays(7)
来源：http://emb.zhiwuduotai.top

[J06] 计算两时间之差
来源：http://ioh.sjlbkw.cn

Py:   (end - start).total_seconds()
来源：http://hqj.hywenlv.cn

PHP:  $end->diff($start)->days;
来源：http://umm.jyoumei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://van.gotoacloud.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://own.meibo888.top

Java: Duration.between(start, end).toSeconds()
来源：http://cpo.zhongyouzk.top

Go:   end.Sub(start).Hours()
来源：http://ubd.bbcook.cn

Ruby: end - start                 # 返回秒数
来源：http://aje.xingfuxueyuan.xyz

C#:   (end - start).TotalSeconds
来源：http://aot.yuxming.cn

[J07] 比较两个日期
来源：http://evn.ehwqpu.com

Py:   d1 < d2;  d1 == d2
来源：http://qha.zhongyouzk.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qag.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://bhd.tian-w.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ksy.cdnleiting.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vnq.shanyushiyangkeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ogq.gotoacloud.top

Ruby: d1 < d2;  d1 == d2
来源：http://zkn.shanyushiyangtech.top

C#:   d1 < d2;  d1 == d2
来源：http://vff.guannengcc.top

[J08] 提取年月日与星期
来源：http://vzw.iojbl.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://caw.fengsongda.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rlk.hysaishi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ntk.hongshengwenyu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jqg.vqdsnc.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vjs.feifeiyinyue.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://esy.cqqwz.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fsk.jiagoushi.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tfg.yuxming.cn

[J09] 时区处理
来源：http://nab.ppjwa.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jec.shangyingyoupin.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bjx.wangdashe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ucw.jinqigfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qoi.sxryk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pif.yanxiufei.cn


<!-- 参考信息 -->