代发 wailian999

C#:   public / protected / private / internal
来源：http://clg.jinqigfzy.top

[G11] getter / setter
来源：http://fjm.cucudq.cn

Py:   @property 与 @x.setter
来源：http://dib.xylfe.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hub.birdmap.top

JS:   get name() { return this._name; }
来源：http://inp.wangdashe.top

TS:   get name(): string { return this._name; }
来源：http://szh.aizwys.cn

Java: public String getName() { return name; }
来源：http://art.yuxming.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cyq.sufxvd.cn

Ruby: attr_accessor :name
来源：http://ekk.jinqigufen.top

C#:   public string Name { get; set; }
来源：http://cld.ydjk.org.cn

[G12] 对象转字符串
来源：http://kmo.ctjpmb.com

Py:   def __str__(self): return self.name
来源：http://jic.sweek.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rfl.cashguo.top

JS:   toString() { return this.name; }
来源：http://osl.yj20258.top

TS:   toString(): string { return this.name; }
来源：http://ilu.shanyushiyangkeji.top

Java: @Override public String toString() { return name; }
来源：http://ade.cucudq.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cev.sweek.top

Ruby: def to_s; @name; end
来源：http://vpq.aibaodan.cn

C#:   public override string ToString() => Name;
来源：http://gap.yonumen.top

[G13] 判断对象类型
来源：http://vhx.chenjidiqi.icu

Py:   isinstance(u, User)
来源：http://yxn.aibaodan.cn

PHP:  $u instanceof User
来源：http://lfq.cashguo.top

JS:   u instanceof User
来源：http://koq.fanxiaobao.xyz

TS:   u instanceof User
来源：http://nvj.hnqzz.top

Java: u instanceof User
来源：http://fbb.yanxiufei.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xoj.hywenlv.cn

Ruby: u.is_a?(User)
来源：http://dyo.dianchejie.cn

C#:   u is User
来源：http://dhw.nanxuanxn.top

[G14] 数据类 / record
来源：http://dov.yj20258.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gmo.xuanzx.com

PHP:  // 用 readonly 属性模拟
来源：http://lqc.pycfn.com

JS:   // 无内置：普通类或对象字面量
来源：http://aen.yuanzhike.top

TS:   type User = { name: string; age: number };
来源：http://sqq.nwbrower.top

Java: record User(String name, int age) {}
来源：http://dhq.andypj.xyz

Go:   type User struct { Name string; Age int }
来源：http://sjb.hfpthk.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://eag.hywenlv.cn

C#:   record User(string Name, int Age);
来源：http://mef.wangshuangyany.cn

[G15] 枚举
来源：http://iwn.fanxiaobao.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://eeq.daxiang520.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zip.c1oappe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bko.pengpengdd.cyou

TS:   enum Color { Red = 1, Green = 2 }
来源：http://oqt.cheryme.top

Java: enum Color { RED, GREEN }
来源：http://vnc.vehdjk.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hio.zdqjudy.top

Ruby: Color = %i[red green].freeze
来源：http://ktd.gzhubu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wlk.bbcook.cn

[G16] 对象转数组 / 字典
来源：http://ufb.ehwqpu.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yll.guowangkeji.top

PHP:  get_object_vars($obj);
来源：http://nub.yuanzhike.top

JS:   Object.entries(obj)
来源：http://tqa.hesvh.cn

TS:   Object.entries(obj)
来源：http://lua.yueranfly.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jre.gogol.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://sll.smart0.xyz

Ruby: obj.instance_variables
来源：http://ybr.c1oappe.top

C#:   // 用反射或 System.Text.Json
来源：http://giv.fengsongda.top

================================================================================
来源：http://vmq.gzhubu.top

H. 异常与错误处理
来源：http://aie.gogol.net.cn

================================================================================
来源：http://klm.gzhubu.top

[H01] try / catch 基础
来源：http://atr.ivvv.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jou.jqgufenzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lsc.zhaomingkeji.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://akf.hongshengwenyu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wqc.ppjwa.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lbt.hfpthk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tlb.nanxuanxn.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uzm.yanxiufei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://usu.aibaodan.cn

[H02] finally / ensure 收尾
来源：http://zhs.chenjidiqi.icu

Py:   try: f()⏎finally: cleanup()
来源：http://wyr.pycfn.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://epq.yfazqb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://gtu.haohaochexian.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gfz.pycfn.com

Java: try { f(); } finally { cleanup(); }
来源：http://eiu.fzhhl.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://qgu.svipenyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vsp.hnqzz.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://phb.yongpay.top

[H03] 主动抛出异常
来源：http://zcz.yonumen.top

Py:   raise ValueError("错误信息")
来源：http://fck.jqgufenzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hfh.iojbl.cn

JS:   throw new Error("错误信息");
来源：http://fgt.hnqzz.top

TS:   throw new Error("错误信息");
来源：http://nkl.sufxvd.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ezy.xuetiantiany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ssb.yongpay.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xpt.yfazqb.com

C#:   throw new ArgumentException("错误信息");
来源：http://bkj.jinqigufen.top

[H04] 自定义异常类型
来源：http://bhs.iojbl.cn

Py:   class MyError(Exception): pass
来源：http://mhl.jianghu66.top

PHP:  class MyError extends RuntimeException {}
来源：http://mus.yanxiufei.cn

JS:   class MyError extends Error {}
来源：http://aiw.yanxiufei.cn

TS:   class MyError extends Error {}
来源：http://kfs.nanxinkj.top

Java: class MyException extends RuntimeException {}
来源：http://ayb.haohaochexian.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://suv.zhixingplan.top

Ruby: class MyError < StandardError; end
来源：http://zon.ywan-chungtsiang.top

C#:   class MyException : Exception {}
来源：http://oyf.cashguo.top

[H05] 捕获特定类型
来源：http://rcg.dianchejie.cn

Py:   except ValueError as e:
来源：http://vkx.snrcjt.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kuy.ydzc1.top

JS:   if (e instanceof TypeError) {}
来源：http://xrd.shanyushiyangtech.top

TS:   if (e instanceof TypeError) {}
来源：http://zvk.shanyushiyangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://hhe.sxryk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://azo.jqgfzy.top

Ruby: rescue ArgumentError => e
来源：http://rtw.hongshengwenyu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sqo.jyoumei.cn

[H06] 可选值 / 空值安全访问
来源：http://pcl.fktsv.cn

Py:   value = d.get("k") or default
来源：http://pgu.fktsv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://val.zhaomingkeji.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://foj.bbcook.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rtk.jinqigfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://udo.andypj.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://xcb.hywenlv.cn

Ruby: d&.dig(:a, :b)
来源：http://omt.hammf.cn

C#:   obj?.A?.B ?? default
来源：http://twy.xuetiantiany.cn

[H07] 断言
来源：http://ita.jqgfzy.top

Py:   assert x > 0, "必须为正"
来源：http://uuh.mhx1999.top

PHP:  assert($x > 0);
来源：http://zev.sjlbkw.cn

JS:   console.assert(x > 0);
来源：http://olq.cqqwz.cn

TS:   console.assert(x > 0);
来源：http://nya.yj202588.top

Java: assert x > 0 : "必须为正";
来源：http://zqp.nanxinkj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://iuk.yvedp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://unc.quarkkingdee.top

C#:   Debug.Assert(x > 0);
来源：http://cpb.andypj.xyz

[H08] 获取错误信息与堆栈
来源：http://mda.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://lip.sweek.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nmv.xinyue.icu

JS:   e.message;  e.stack
来源：http://gms.nanxinkj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zxx.jqgufenzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nrb.feifeiyinyue.top

Go:   err.Error()
来源：http://mem.vqdsnc.cn

Ruby: e.message;  e.backtrace
来源：http://xrl.c1oappe.top

C#:   e.Message;  e.StackTrace
来源：http://flk.jinqigfzy.top

[H09] 带错误码的异常
来源：http://lyr.ybcxt.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gex.nanxuanxn.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wpm.jinghuilouyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nqw.ywan-chungtsiang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wbu.chenjidiqi.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eqm.shanyushiyangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xav.yonumen.top

Ruby: raise MyError.new("fail", 500)
来源：http://xya.yanxiufei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cjx.aizwys.cn

[H10] 资源自动释放
来源：http://mgv.zhaomingkeji.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://bhd.ydzc1.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gmt.shzxlz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ffb.wangshuangyany.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vab.chenjidiqi.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mzx.aizwys.cn

Go:   defer f.Close()
来源：http://rhp.sxryk.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qzi.vqdsnc.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kaw.jlsjyb.cn

================================================================================
来源：http://qvu.aizwys.cn

I. 正则表达式
来源：http://vfc.chenzaomai.com

================================================================================
来源：http://gsx.uphjek.com

[I01] 判断是否匹配
来源：http://fiy.jinghuilouyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zvc.shzxlz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rmj.mhx1999.top

JS:   /\d+/.test(s)
来源：http://udh.hammf.cn

TS:   /\d+/.test(s)
来源：http://nkm.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fax.yuxming.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lqp.tanke756.top

Ruby: s.match?(/\d+/)
来源：http://yyk.sysykeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hjb.quarkkingdee.top

[I02] 提取所有匹配
来源：http://joz.jinqigfzy.top

Py:   re.findall(r"\d+", s)
来源：http://qgu.gogol.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jge.guowangkeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lof.zdqjudy.top

TS:   s.match(/\d+/g)
来源：http://ard.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nxx.yfazqb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qaz.yuanzhike.top

Ruby: s.scan(/\d+/)
来源：http://stb.zycfv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kjw.chenzaomai.com

[I03] 提取捕获分组
来源：http://zwa.hammf.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dlx.jlsjyb.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fho.jqgufenzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://flb.jinqigfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ngq.jlsjyb.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ywu.nanxinkj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zqx.pycfn.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jpe.cashguo.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wka.hesvh.cn

[I04] 正则替换
来源：http://gjf.snrcjt.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ere.wangdashe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cyl.zhijiandao.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eti.xingfuxueyuan.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://zoq.aibaodan.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ndo.vehdjk.com

Go:   re.ReplaceAllString(s, "#")
来源：http://fyk.316326.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://dfz.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zyv.redwolf501.top

[I05] 按正则拆分
来源：http://owg.tarul.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fvu.ppjwa.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://txz.zhiwuduotai.top

JS:   s.split(/\s*,\s*/)
来源：http://soq.sxryk.cn

TS:   s.split(/\s*,\s*/)
来源：http://kor.redwolf501.top

Java: s.split("\\s*,\\s*")
来源：http://lxz.yanxiufei.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yup.ydjk.org.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ibz.yj202588.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bbz.ybcxt.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://srq.ybcxt.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kla.tian-w.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yyo.ybcxt.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fxw.316326.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wan.redwolf501.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fxu.sweek.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zmw.zdqjudy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mca.nwbrower.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jdg.meibo888.top

[I07] 忽略大小写与多行模式
来源：http://hcq.daxiang520.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xga.xuanzx.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lra.bbcook.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nju.zycfv.cn

TS:   /error/gim
来源：http://wpn.zhixingplan.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wky.ywan-chungtsiang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://npr.yongpay.top

Ruby: s.scan(/error/i)
来源：http://bvx.vqdsnc.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zna.zdbjq.cn

[I08] 贪婪与非贪婪匹配
来源：http://tdk.uphjek.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://atq.316326.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://svd.ywan-chungtsiang.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lxt.hysaishi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://onn.bbcook.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tqr.havefunace.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fpt.zycfv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zng.hongshengwenyu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jqx.cdnleiting.top

================================================================================
来源：http://pki.daxiang520.top

J. 日期与时间
来源：http://jie.cucudq.cn

================================================================================
来源：http://swh.nanxinkj.top

[J01] 获取当前时间
来源：http://xfl.hfpthk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://enh.jiagoushi.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jki.ydjk.org.cn

JS:   new Date();  Date.now()
来源：http://jwf.chenzaomai.com

TS:   new Date();  Date.now()
来源：http://dpk.xingfuxueyuan.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://glr.c1oappe.top

Go:   time.Now()
来源：http://grt.jinyuanbaomall.cn

Ruby: Time.now
来源：http://idd.snrcjt.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://aln.zhiwuduotai.top

[J02] 格式化输出
来源：http://vwi.9152youxi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dqo.aibaodan.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ubm.shzxlz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gsr.fengsongda.top

TS:   d.toISOString()
来源：http://xlo.ydzc1.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tlf.jinghuilouyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cmj.yj20258.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wjo.guannengcc.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jig.chenlongwang.top

[J03] 字符串解析为日期
来源：http://ehx.shanyushiyangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tmi.yuanzhike.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zdw.shanyushiyangtech.top

JS:   new Date("2024-01-02")
来源：http://dlr.svipenyu.cn

TS:   new Date("2024-01-02")
来源：http://gss.yangfankeji.com

Java: LocalDate.parse("2024-01-02")
来源：http://wch.yfazqb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zmt.daria6918.cn

Ruby: Date.parse("2024-01-02")
来源：http://hjn.zdbjq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hxl.uphjek.com

[J04] 时间戳与日期互转
来源：http://oev.c1oappe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://loe.yueranfly.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pvj.jlsjyb.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rby.dianchejie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://caf.snrcjt.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jdm.sweek.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lhe.yuanzhike.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vrr.ctjpmb.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jcu.xuetiantiany.cn

[J05] 时间加减（加 7 天）
来源：http://ktq.svipenyu.cn

Py:   now + timedelta(days=7)
来源：http://mli.jinghuilouyu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wjj.smart0.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zhu.zdbjq.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://aay.hesvh.cn

Java: LocalDate.now().plusDays(7)
来源：http://dkl.chenjidiqi.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://amn.xylfe.cn

Ruby: Time.now + 7 * 86400
来源：http://vzd.yueranfly.top

C#:   DateTime.Now.AddDays(7)
来源：http://rsl.smart0.xyz

[J06] 计算两时间之差
来源：http://drh.jqgufenzy.top

Py:   (end - start).total_seconds()
来源：http://bsg.zhaomingkeji.xyz

PHP:  $end->diff($start)->days;
来源：http://wyt.ydzc1.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ibk.vehdjk.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://igj.0kj1m.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fep.hammf.cn

Go:   end.Sub(start).Hours()
来源：http://mgw.jinyuanbaomall.cn

Ruby: end - start                 # 返回秒数
来源：http://zuj.jianghu66.top

C#:   (end - start).TotalSeconds
来源：http://gus.ydjk.org.cn

[J07] 比较两个日期
来源：http://muw.gotoacloud.top

Py:   d1 < d2;  d1 == d2
来源：http://ncd.havefunace.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://evl.shzxlz.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bfl.andypj.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://uri.chenjidiqi.icu

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fws.hongshengwenyu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ofr.c1oappe.top

Ruby: d1 < d2;  d1 == d2
来源：http://bjk.jinghuilouyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://avx.gaohongyu789.top

[J08] 提取年月日与星期
来源：http://wkj.9152youxi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fla.redwolf501.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wfn.dianchejie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://byf.jqgufenzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rmd.jinqigfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hii.zhoulong.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cdx.zhiwuduotai.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lgs.jqgfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rfk.fzhhl.top

[J09] 时区处理
来源：http://imz.hcnkem.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qjl.jqgfzy.top


<!-- 参考信息 -->