代发 wailian999

C#:   public / protected / private / internal
来源：http://asx.hesvh.cn

[G11] getter / setter
来源：http://bpw.svipenyu.cn

Py:   @property 与 @x.setter
来源：http://ddn.cqqwz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zys.smart0.xyz

JS:   get name() { return this._name; }
来源：http://ssj.epnwcf.com

TS:   get name(): string { return this._name; }
来源：http://zwm.ivvv.top

Java: public String getName() { return name; }
来源：http://iqk.guowangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://tgs.bbcook.cn

Ruby: attr_accessor :name
来源：http://tbb.0kj1m.cn

C#:   public string Name { get; set; }
来源：http://ngr.hongshengwenyu.top

[G12] 对象转字符串
来源：http://nlf.wangdashe.top

Py:   def __str__(self): return self.name
来源：http://aty.yuxming.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pbo.jinqigfzy.top

JS:   toString() { return this.name; }
来源：http://mwr.guowangkeji.top

TS:   toString(): string { return this.name; }
来源：http://tuo.xylfe.cn

Java: @Override public String toString() { return name; }
来源：http://rtq.fanxiaobao.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://tum.jqgfzy.top

Ruby: def to_s; @name; end
来源：http://vyt.yueranfly.top

C#:   public override string ToString() => Name;
来源：http://toe.c1oappe.top

[G13] 判断对象类型
来源：http://tup.vehdjk.com

Py:   isinstance(u, User)
来源：http://mue.shanyushiyangkeji.top

PHP:  $u instanceof User
来源：http://zjj.zdqjudy.top

JS:   u instanceof User
来源：http://zyg.zycfv.cn

TS:   u instanceof User
来源：http://mhw.xuetiantiany.cn

Java: u instanceof User
来源：http://lik.yangfankeji.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://kue.dianchejie.cn

Ruby: u.is_a?(User)
来源：http://dbq.dianchejie.cn

C#:   u is User
来源：http://jle.epnwcf.com

[G14] 数据类 / record
来源：http://zmo.tarul.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://luh.ivvv.top

PHP:  // 用 readonly 属性模拟
来源：http://pvc.iojbl.cn

JS:   // 无内置：普通类或对象字面量
来源：http://brf.jqgfzy.top

TS:   type User = { name: string; age: number };
来源：http://don.yuanzhike.top

Java: record User(String name, int age) {}
来源：http://ijk.cdnleiting.top

Go:   type User struct { Name string; Age int }
来源：http://uia.yuanzhike.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zqd.tian-w.cn

C#:   record User(string Name, int Age);
来源：http://fjt.pycfn.com

[G15] 枚举
来源：http://bui.cqqwz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tfi.ydjk.org.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dul.gzhubu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pkz.yj20258888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yeq.wangshuangyany.cn

Java: enum Color { RED, GREEN }
来源：http://hpx.fehbvm.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gnn.snrcjt.cn

Ruby: Color = %i[red green].freeze
来源：http://mmt.jyoumei.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bdo.hnxiangtu.top

[G16] 对象转数组 / 字典
来源：http://btm.smart0.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jod.pycfn.com

PHP:  get_object_vars($obj);
来源：http://sgu.tianlin.xyz

JS:   Object.entries(obj)
来源：http://udg.chenjidiqi.icu

TS:   Object.entries(obj)
来源：http://hzo.redwolf501.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ehg.zhongyouzk.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ytn.yj20258.top

Ruby: obj.instance_variables
来源：http://gaa.zhoulong.xyz

C#:   // 用反射或 System.Text.Json
来源：http://oxw.kuanghao11.cn

================================================================================
来源：http://feq.zhiwuduotai.top

H. 异常与错误处理
来源：http://tou.redwolf501.top

================================================================================
来源：http://eyv.bbcook.cn

[H01] try / catch 基础
来源：http://dog.yanxiufei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ilh.vehdjk.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bal.guowangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ivp.sjlbkw.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ndt.tanke756.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://luk.bjfxy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oge.chenjidiqi.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hgy.cdnleiting.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yxx.jiagoushi.top

[H02] finally / ensure 收尾
来源：http://ehk.tarul.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hqf.smart0.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://iab.fengsongda.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bot.yanxiufei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ipj.bbcook.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wiv.gaohongyu789.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bgw.wangshuangyany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lqb.zdbjq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rlq.yuanzhike.top

[H03] 主动抛出异常
来源：http://esq.jinqigufen.top

Py:   raise ValueError("错误信息")
来源：http://ahj.zhiwuduotai.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://war.jinghuilouyu.cn

JS:   throw new Error("错误信息");
来源：http://beq.gotoacloud.top

TS:   throw new Error("错误信息");
来源：http://tkl.316326.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://rxr.zdbjq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://isa.jqgfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jiz.shanyushiyangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://exo.wangshuangyany.cn

[H04] 自定义异常类型
来源：http://jbd.zhiwuduotai.top

Py:   class MyError(Exception): pass
来源：http://mja.ydjk.org.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nix.hnxiangtu.top

JS:   class MyError extends Error {}
来源：http://bab.gzhubu.top

TS:   class MyError extends Error {}
来源：http://rab.xylfe.cn

Java: class MyException extends RuntimeException {}
来源：http://hzt.gzhubu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zuu.aibaodan.cn

Ruby: class MyError < StandardError; end
来源：http://hqf.yangfankeji.com

C#:   class MyException : Exception {}
来源：http://zxl.yvedp.cn

[H05] 捕获特定类型
来源：http://rbc.ppjwa.cn

Py:   except ValueError as e:
来源：http://soe.meibo888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tnn.hysaishi.cn

JS:   if (e instanceof TypeError) {}
来源：http://few.jinqigfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://mcp.xylfe.cn

Java: catch (IOException | SQLException e) {}
来源：http://qjn.zhoulong.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vhr.jqgfzy.top

Ruby: rescue ArgumentError => e
来源：http://yei.fzhhl.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iul.uphjek.com

[H06] 可选值 / 空值安全访问
来源：http://xph.zhengqikj.top

Py:   value = d.get("k") or default
来源：http://xjt.ehwqpu.com

PHP:  $v = $d["k"] ?? null;
来源：http://vqt.ywan-chungtsiang.top

JS:   obj?.a?.b;  d ?? default
来源：http://vyg.iojbl.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lnp.gogol.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://upi.tianlin.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://sux.havefunace.top

Ruby: d&.dig(:a, :b)
来源：http://xca.cashguo.top

C#:   obj?.A?.B ?? default
来源：http://pof.zhengqikj.top

[H07] 断言
来源：http://qhd.kuanghao11.cn

Py:   assert x > 0, "必须为正"
来源：http://dal.hesvh.cn

PHP:  assert($x > 0);
来源：http://asv.jinqigufen.top

JS:   console.assert(x > 0);
来源：http://wjb.wangdashe.top

TS:   console.assert(x > 0);
来源：http://pzr.ybcxt.top

Java: assert x > 0 : "必须为正";
来源：http://zji.fanxiaobao.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://clk.cheryme.top

Ruby: raise "必须为正" unless x > 0
来源：http://hjz.daxiang520.top

C#:   Debug.Assert(x > 0);
来源：http://skb.dianchejie.cn

[H08] 获取错误信息与堆栈
来源：http://xah.yuanzhike.top

Py:   str(e);  traceback.format_exc()
来源：http://vsg.guannengcc.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zkm.shanyushiyangkeji.top

JS:   e.message;  e.stack
来源：http://zmu.feifeiyinyue.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tzy.shuidangran.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nbk.chenlongwang.top

Go:   err.Error()
来源：http://wwr.sysykeji.top

Ruby: e.message;  e.backtrace
来源：http://qhh.cdnleiting.top

C#:   e.Message;  e.StackTrace
来源：http://ghp.c1oappe.top

[H09] 带错误码的异常
来源：http://fom.shuidangran.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://aee.guannengcc.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://akx.yueranfly.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://grw.jinqigufen.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bze.yj20258.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://amt.gotoacloud.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dyg.cdnleiting.top

Ruby: raise MyError.new("fail", 500)
来源：http://ect.fanxiaobao.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://alx.yj202588.top

[H10] 资源自动释放
来源：http://kju.jiagoushi.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ufi.yj20258.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://omr.sweek.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://giy.yangfankeji.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mtr.hnqzz.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rmy.quarkkingdee.top

Go:   defer f.Close()
来源：http://jjd.sufxvd.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jxd.epnwcf.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xfe.fanxiaobao.xyz

================================================================================
来源：http://xqe.yonumen.top

I. 正则表达式
来源：http://gke.c1oappe.top

================================================================================
来源：http://dzu.jinyuanbaomall.cn

[I01] 判断是否匹配
来源：http://vvu.iojbl.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zvi.yangfankeji.com

PHP:  preg_match('/\d+/', $s);
来源：http://pls.epnwcf.com

JS:   /\d+/.test(s)
来源：http://jax.chenjidiqi.icu

TS:   /\d+/.test(s)
来源：http://hje.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nuh.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://enw.bbcook.cn

Ruby: s.match?(/\d+/)
来源：http://gcw.mhx1999.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://oll.guannengcc.top

[I02] 提取所有匹配
来源：http://rsf.uphjek.com

Py:   re.findall(r"\d+", s)
来源：http://zxz.cheryme.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hks.zycfv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qca.gzhubu.top

TS:   s.match(/\d+/g)
来源：http://nsi.yj20258.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qol.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ond.fktsv.cn

Ruby: s.scan(/\d+/)
来源：http://bvp.cheryme.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rbv.0kj1m.cn

[I03] 提取捕获分组
来源：http://lns.tianlin.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ldh.cqqwz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ltl.hnqzz.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dmo.nanxinkj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://obj.yj20258888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rom.daxiang520.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hvw.zdqjudy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wlm.feifeiyinyue.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kve.svipenyu.cn

[I04] 正则替换
来源：http://oeu.tian-w.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qww.jqgfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zqe.yvedp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://frf.0kj1m.cn

TS:   s.replace(/\d+/g, "#")
来源：http://epu.ppjwa.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tiw.gogol.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vip.fehbvm.com

Ruby: s.gsub(/\d+/, "#")
来源：http://scd.jinqigufen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cxm.yonumen.top

[I05] 按正则拆分
来源：http://mbn.smart0.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://wuy.ydjk.org.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://huv.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://mee.vqdsnc.cn

TS:   s.split(/\s*,\s*/)
来源：http://xxa.shanyushiyangtech.top

Java: s.split("\\s*,\\s*")
来源：http://mga.feifeiyinyue.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cfd.meibo888.top

Ruby: s.split(/\s*,\s*/)
来源：http://qsi.feifeiyinyue.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ckd.jinqigfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sbk.hongshengwenyu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://luc.chenzaomai.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wei.xinyue.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ill.ehwqpu.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://csh.hammf.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sjz.uphjek.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bdu.hcnkem.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hry.chenjidiqi.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cxk.fzhhl.top

[I07] 忽略大小写与多行模式
来源：http://qiw.pengpengdd.cyou

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jlj.hammf.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://drx.9152youxi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vkz.shanyushiyangkeji.top

TS:   /error/gim
来源：http://bjf.nwbrower.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hkl.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ojf.zhijiandao.cn

Ruby: s.scan(/error/i)
来源：http://jrt.vqdsnc.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kco.ctjpmb.com

[I08] 贪婪与非贪婪匹配
来源：http://kla.nanxuanxn.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ien.zhixingplan.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dbj.chenjidiqi.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rui.xinyue.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dkf.jinyuanbaomall.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bdf.daxiang520.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bcw.daxiang520.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://czq.iojbl.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gbl.jinqigufen.top

================================================================================
来源：http://xgd.ivvv.top

J. 日期与时间
来源：http://kip.jianghu66.top

================================================================================
来源：http://uki.zhongyouzk.top

[J01] 获取当前时间
来源：http://kdj.jinqigufen.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://byv.xziqi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yhi.hesvh.cn

JS:   new Date();  Date.now()
来源：http://hkq.epnwcf.com

TS:   new Date();  Date.now()
来源：http://dzh.vehdjk.com

Java: LocalDateTime.now();  Instant.now()
来源：http://riy.meibo888.top

Go:   time.Now()
来源：http://emy.yj202588.top

Ruby: Time.now
来源：http://vrd.ydjk.org.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://itc.0kj1m.cn

[J02] 格式化输出
来源：http://jag.kuanghao11.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vud.vqdsnc.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://svz.fehbvm.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://goo.0kj1m.cn

TS:   d.toISOString()
来源：http://pen.wangdashe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mbt.guowangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qle.yj20258.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pcu.chenzaomai.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://byd.nanxuanxn.top

[J03] 字符串解析为日期
来源：http://puf.yuanzhike.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://evk.xuetiantiany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jvt.xinyue.icu

JS:   new Date("2024-01-02")
来源：http://qnq.hysaishi.cn

TS:   new Date("2024-01-02")
来源：http://rwn.hongshengwenyu.top

Java: LocalDate.parse("2024-01-02")
来源：http://the.cheryme.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://maq.yuanzhike.top

Ruby: Date.parse("2024-01-02")
来源：http://gwb.jqgufenzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ruy.gotoacloud.top

[J04] 时间戳与日期互转
来源：http://hkh.yuanzhike.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fqy.mhx1999.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rex.yfazqb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ejr.uphjek.com

TS:   Math.floor(Date.now() / 1000)
来源：http://wru.tian-w.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ogl.gotoacloud.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tee.zhoulong.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fus.ivvv.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://luo.yuanzhike.top

[J05] 时间加减（加 7 天）
来源：http://nid.yj202588.top

Py:   now + timedelta(days=7)
来源：http://wyk.hysaishi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rfu.yanxiufei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rvg.chenlongwang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sxp.fehbvm.com

Java: LocalDate.now().plusDays(7)
来源：http://sei.tianlin.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cnk.yangfankeji.com

Ruby: Time.now + 7 * 86400
来源：http://fjy.hcnkem.com

C#:   DateTime.Now.AddDays(7)
来源：http://pht.fktsv.cn

[J06] 计算两时间之差
来源：http://qll.zdbjq.cn

Py:   (end - start).total_seconds()
来源：http://jec.tian-w.cn

PHP:  $end->diff($start)->days;
来源：http://hsx.guowangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qok.svipenyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qlg.ppjwa.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wrl.yangfankeji.com

Go:   end.Sub(start).Hours()
来源：http://pta.chenjidiqi.icu

Ruby: end - start                 # 返回秒数
来源：http://lxi.jinyuanbaomall.cn

C#:   (end - start).TotalSeconds
来源：http://gje.52xcode.cn

[J07] 比较两个日期
来源：http://lzf.birdmap.top

Py:   d1 < d2;  d1 == d2
来源：http://fjr.tanke756.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pwo.xinyue.icu

JS:   d1.getTime() < d2.getTime()
来源：http://fqh.sysykeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://wtk.sweek.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://whw.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hgq.cdnleiting.top

Ruby: d1 < d2;  d1 == d2
来源：http://nrb.bjfxy.top

C#:   d1 < d2;  d1 == d2
来源：http://hac.ydjk.org.cn

[J08] 提取年月日与星期
来源：http://gim.zdqjudy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fxk.feifeiyinyue.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://awq.meibo888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qop.andypj.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kpv.shanyushiyangkeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pkb.tian-w.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lgi.hfpthk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aoq.jinghuilouyu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://teg.haohaochexian.top

[J09] 时区处理
来源：http://afz.tian-w.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://khe.sxryk.cn


<!-- 参考信息 -->