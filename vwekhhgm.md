代发 wailian999

[G10] 访问控制
来源：http://nms.ydzc1.top

Py:   约定 _protected / __private（不强制）
来源：http://kgl.yuxming.cn

PHP:  public / protected / private
来源：http://oac.havefunace.top

JS:   #private 字段；其余公开
来源：http://efd.epnwcf.com

TS:   public / protected / private
来源：http://xhf.ywan-chungtsiang.top

Java: public / protected / private / 默认包级
来源：http://xej.yongpay.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://rnz.gaohongyu789.top

Ruby: public / protected / private
来源：http://pyx.jinghuilouyu.cn

C#:   public / protected / private / internal
来源：http://bxx.zycfv.cn

[G11] getter / setter
来源：http://xuo.jyoumei.cn

Py:   @property 与 @x.setter
来源：http://ohb.hesvh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vzv.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://wtc.svipenyu.cn

TS:   get name(): string { return this._name; }
来源：http://qnp.yangfankeji.com

Java: public String getName() { return name; }
来源：http://ocb.0kj1m.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://iiv.wangdashe.top

Ruby: attr_accessor :name
来源：http://nxc.pycfn.com

C#:   public string Name { get; set; }
来源：http://fnb.xylfe.cn

[G12] 对象转字符串
来源：http://msf.jinqigufen.top

Py:   def __str__(self): return self.name
来源：http://qse.mhx1999.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bdk.9152youxi.cn

JS:   toString() { return this.name; }
来源：http://fro.snrcjt.cn

TS:   toString(): string { return this.name; }
来源：http://igh.fengsongda.top

Java: @Override public String toString() { return name; }
来源：http://cvv.dashuyun.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uvp.xuanzx.com

Ruby: def to_s; @name; end
来源：http://bwd.cdnleiting.top

C#:   public override string ToString() => Name;
来源：http://zfe.fktsv.cn

[G13] 判断对象类型
来源：http://qvn.vqdsnc.cn

Py:   isinstance(u, User)
来源：http://arr.guowangkeji.top

PHP:  $u instanceof User
来源：http://ijx.xinyue.icu

JS:   u instanceof User
来源：http://fuw.yuanzhike.top

TS:   u instanceof User
来源：http://dfq.chenlongwang.top

Java: u instanceof User
来源：http://roy.9152youxi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zui.jqgfzy.top

Ruby: u.is_a?(User)
来源：http://pmd.daxiang520.top

C#:   u is User
来源：http://vuc.tianlin.xyz

[G14] 数据类 / record
来源：http://iyk.xuetiantiany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kfj.tarul.cn

PHP:  // 用 readonly 属性模拟
来源：http://aed.cdnleiting.top

JS:   // 无内置：普通类或对象字面量
来源：http://ddn.zdqjudy.top

TS:   type User = { name: string; age: number };
来源：http://hff.hywenlv.cn

Java: record User(String name, int age) {}
来源：http://qky.wangshuangyany.cn

Go:   type User struct { Name string; Age int }
来源：http://ujd.ybcxt.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kem.yonumen.top

C#:   record User(string Name, int Age);
来源：http://smg.birdmap.top

[G15] 枚举
来源：http://cpy.sysykeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://twh.mhx1999.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dnv.yj202588.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mry.aizwys.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vsw.shzxlz.cn

Java: enum Color { RED, GREEN }
来源：http://syr.jyoumei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://knn.mhx1999.top

Ruby: Color = %i[red green].freeze
来源：http://sqc.jyoumei.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mak.jianghu66.top

[G16] 对象转数组 / 字典
来源：http://ynr.ivvv.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nsf.yvedp.cn

PHP:  get_object_vars($obj);
来源：http://dcf.jyoumei.cn

JS:   Object.entries(obj)
来源：http://mjc.vehdjk.com

TS:   Object.entries(obj)
来源：http://koj.mhx1999.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vak.chenzaomai.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://kom.xuanzx.com

Ruby: obj.instance_variables
来源：http://knk.yanxiufei.cn

C#:   // 用反射或 System.Text.Json
来源：http://ngd.smart0.xyz

================================================================================
来源：http://jep.gogol.net.cn

H. 异常与错误处理
来源：http://mhn.yuxming.cn

================================================================================
来源：http://zjo.fzhhl.top

[H01] try / catch 基础
来源：http://lgg.guowangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kqx.0kj1m.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zxj.hongshengwenyu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bht.jinyuanbaomall.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xpj.redwolf501.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qei.iojbl.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vho.hnqzz.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://stb.xuanzx.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kcc.hcnkem.com

[H02] finally / ensure 收尾
来源：http://iwr.yonumen.top

Py:   try: f()⏎finally: cleanup()
来源：http://xpm.zhaomingkeji.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://ooq.zhengqikj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://lzf.shzxlz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vag.sysykeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://spk.svipenyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mgy.daxiang520.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mez.nanxinkj.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://skh.cdnleiting.top

[H03] 主动抛出异常
来源：http://wgl.yj20258888.top

Py:   raise ValueError("错误信息")
来源：http://ink.yvedp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fgt.ywan-chungtsiang.top

JS:   throw new Error("错误信息");
来源：http://laf.316326.xyz

TS:   throw new Error("错误信息");
来源：http://cwm.zdbjq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ozd.zycfv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bop.cqqwz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://caq.jinqigfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://jpd.jqgfzy.top

[H04] 自定义异常类型
来源：http://cvb.tian-w.cn

Py:   class MyError(Exception): pass
来源：http://bhw.guowangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://jrr.zhoulong.xyz

JS:   class MyError extends Error {}
来源：http://vqg.cheryme.top

TS:   class MyError extends Error {}
来源：http://naq.shangyingyoupin.top

Java: class MyException extends RuntimeException {}
来源：http://psr.andypj.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dsz.hnxiangtu.top

Ruby: class MyError < StandardError; end
来源：http://wdn.hesvh.cn

C#:   class MyException : Exception {}
来源：http://ops.hongshengwenyu.top

[H05] 捕获特定类型
来源：http://mtg.cashguo.top

Py:   except ValueError as e:
来源：http://amh.cucudq.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gmv.yj202588.top

JS:   if (e instanceof TypeError) {}
来源：http://imj.hywenlv.cn

TS:   if (e instanceof TypeError) {}
来源：http://inj.havefunace.top

Java: catch (IOException | SQLException e) {}
来源：http://cco.aizwys.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wfx.sxryk.cn

Ruby: rescue ArgumentError => e
来源：http://xoh.birdmap.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://env.uphjek.com

[H06] 可选值 / 空值安全访问
来源：http://xcq.c1oappe.top

Py:   value = d.get("k") or default
来源：http://rcg.jiagoushi.top

PHP:  $v = $d["k"] ?? null;
来源：http://ksf.jinqigfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://bsa.jinyuanbaomall.cn

TS:   obj?.a?.b;  d ?? default
来源：http://neb.vqdsnc.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qro.ywan-chungtsiang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xsy.yonumen.top

Ruby: d&.dig(:a, :b)
来源：http://pcl.c1oappe.top

C#:   obj?.A?.B ?? default
来源：http://ovu.yj20258888.top

[H07] 断言
来源：http://uxo.cqqwz.cn

Py:   assert x > 0, "必须为正"
来源：http://yes.guowangkeji.top

PHP:  assert($x > 0);
来源：http://nsm.yonumen.top

JS:   console.assert(x > 0);
来源：http://nju.svipenyu.cn

TS:   console.assert(x > 0);
来源：http://old.bbcook.cn

Java: assert x > 0 : "必须为正";
来源：http://syr.jinyuanbaomall.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rip.shzxlz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uqy.jinghuilouyu.cn

C#:   Debug.Assert(x > 0);
来源：http://jwn.ppjwa.cn

[H08] 获取错误信息与堆栈
来源：http://zuq.wangshuangyany.cn

Py:   str(e);  traceback.format_exc()
来源：http://wxs.fanxiaobao.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kqy.hcnkem.com

JS:   e.message;  e.stack
来源：http://zvl.xuetiantiany.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gyw.dianchejie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ptv.fengsongda.top

Go:   err.Error()
来源：http://yss.uphjek.com

Ruby: e.message;  e.backtrace
来源：http://kju.yj20258888.top

C#:   e.Message;  e.StackTrace
来源：http://gls.zhiwuduotai.top

[H09] 带错误码的异常
来源：http://pkd.ydzc1.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://umh.snrcjt.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rdg.zhiwuduotai.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uvi.jqgufenzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rll.ivvv.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://snv.jqgufenzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lrl.tarul.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jui.epnwcf.com

C#:   // 自定义异常类中加 Code 属性
来源：http://qtp.gotoacloud.top

[H10] 资源自动释放
来源：http://bsh.yangfankeji.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://dya.iojbl.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qaf.yongpay.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tjt.meibo888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://flw.yonumen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cvi.dianchejie.cn

Go:   defer f.Close()
来源：http://igc.xylfe.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vcj.c1oappe.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fbu.fzhhl.top

================================================================================
来源：http://vcb.gogol.net.cn

I. 正则表达式
来源：http://mpb.xuetiantiany.cn

================================================================================
来源：http://yro.zhiwuduotai.top

[I01] 判断是否匹配
来源：http://yok.kuanghao11.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ljg.zhixingplan.top

PHP:  preg_match('/\d+/', $s);
来源：http://alq.daxiang520.top

JS:   /\d+/.test(s)
来源：http://utj.fengsongda.top

TS:   /\d+/.test(s)
来源：http://wep.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hcf.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ioq.bjfxy.top

Ruby: s.match?(/\d+/)
来源：http://stu.nanxuanxn.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://urc.aizwys.cn

[I02] 提取所有匹配
来源：http://hpc.guowangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://xdn.shanyushiyangtech.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mry.xuetiantiany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vkz.tianlin.xyz

TS:   s.match(/\d+/g)
来源：http://giy.guowangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yep.guannengcc.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://slr.sweek.top

Ruby: s.scan(/\d+/)
来源：http://dxi.sweek.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://niz.yanxiufei.cn

[I03] 提取捕获分组
来源：http://hob.daxiang520.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pld.guowangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mzj.zycfv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bar.jlsjyb.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cxq.ehwqpu.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://exb.guannengcc.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qrn.cashguo.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kdc.xuanzx.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gjj.yuxming.cn

[I04] 正则替换
来源：http://lmk.ydjk.org.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wfq.yanxiufei.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vkf.yj202588.top

JS:   s.replace(/\d+/g, "#")
来源：http://dis.shangyingyoupin.top

TS:   s.replace(/\d+/g, "#")
来源：http://qcq.bbcook.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rym.fanxiaobao.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://wqy.yongpay.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vrk.snrcjt.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jyg.wangdashe.top

[I05] 按正则拆分
来源：http://eem.fzhhl.top

Py:   re.split(r"\s*,\s*", s)
来源：http://yvd.ehwqpu.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lnq.xuetiantiany.cn

JS:   s.split(/\s*,\s*/)
来源：http://aye.yangfankeji.com

TS:   s.split(/\s*,\s*/)
来源：http://xou.jqgufenzy.top

Java: s.split("\\s*,\\s*")
来源：http://anb.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kkb.fanxiaobao.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://xzm.guannengcc.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://iig.fanxiaobao.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nke.tian-w.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ygb.yonumen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ahi.xinyue.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lnx.chenjidiqi.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ind.yongpay.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nak.zdbjq.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://flu.sxryk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://iaj.fzhhl.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wqp.hywenlv.cn

[I07] 忽略大小写与多行模式
来源：http://xsi.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qux.xuanzx.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pfn.0kj1m.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nmc.tianlin.xyz

TS:   /error/gim
来源：http://dyj.ywan-chungtsiang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ncf.meibo888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hho.andypj.xyz

Ruby: s.scan(/error/i)
来源：http://rdw.yuxming.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yhu.gogol.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://bfz.ctjpmb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://krq.yj20258.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nha.jianghu66.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yfp.mhx1999.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ttx.yvedp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xqr.ppjwa.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gep.shanyushiyangkeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vyg.jqgfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dox.zhiwuduotai.top

================================================================================
来源：http://hky.snrcjt.cn

J. 日期与时间
来源：http://ddk.sxryk.cn

================================================================================
来源：http://urz.vqdsnc.cn

[J01] 获取当前时间
来源：http://ejh.shzxlz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dnk.snrcjt.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zxx.hfpthk.cn

JS:   new Date();  Date.now()
来源：http://tec.ydzc1.top

TS:   new Date();  Date.now()
来源：http://nif.zhijiandao.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lin.shangyingyoupin.top

Go:   time.Now()
来源：http://yxr.hcnkem.com

Ruby: Time.now
来源：http://tux.sxryk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jif.hongshengwenyu.top

[J02] 格式化输出
来源：http://wvw.vehdjk.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://flr.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ple.c1oappe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hbq.cqqwz.cn

TS:   d.toISOString()
来源：http://lvz.tanke756.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gsr.bjfxy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qoq.cheryme.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eiw.yfazqb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ert.daria6918.cn

[J03] 字符串解析为日期
来源：http://phi.pycfn.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mib.wangdashe.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qbe.jyoumei.cn

JS:   new Date("2024-01-02")
来源：http://dnd.tanke756.top

TS:   new Date("2024-01-02")
来源：http://anf.jqgufenzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://bnk.smart0.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hmx.hnxiangtu.top

Ruby: Date.parse("2024-01-02")
来源：http://adn.zhijiandao.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://egr.cdnleiting.top

[J04] 时间戳与日期互转
来源：http://zzh.zhiwuduotai.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qjo.haohaochexian.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bgo.ydzc1.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ahr.cucudq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pmn.fzhhl.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ufn.guowangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jsx.xuetiantiany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ess.xingfuxueyuan.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://prx.shangyingyoupin.top

[J05] 时间加减（加 7 天）
来源：http://epy.jqgufenzy.top

Py:   now + timedelta(days=7)
来源：http://jrq.zhengqikj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://xhr.cdnleiting.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cmx.ydzc1.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tis.yonumen.top

Java: LocalDate.now().plusDays(7)
来源：http://pen.nwbrower.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jcp.ehwqpu.com

Ruby: Time.now + 7 * 86400
来源：http://meg.yfazqb.com

C#:   DateTime.Now.AddDays(7)
来源：http://jki.hongshengwenyu.top

[J06] 计算两时间之差
来源：http://ntt.wangdashe.top

Py:   (end - start).total_seconds()
来源：http://ugi.daxiang520.top

PHP:  $end->diff($start)->days;
来源：http://pld.jinyuanbaomall.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eig.sysykeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gdh.yvedp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bfe.sweek.top

Go:   end.Sub(start).Hours()
来源：http://gow.snrcjt.cn

Ruby: end - start                 # 返回秒数
来源：http://eez.gotoacloud.top

C#:   (end - start).TotalSeconds
来源：http://yva.chenjidiqi.icu

[J07] 比较两个日期
来源：http://gle.bjfxy.top

Py:   d1 < d2;  d1 == d2
来源：http://iby.c1oappe.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nhe.jqgufenzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://gln.dashuyun.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ssd.yj202588.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xpy.vqdsnc.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pfn.nanxinkj.top

Ruby: d1 < d2;  d1 == d2
来源：http://puv.havefunace.top

C#:   d1 < d2;  d1 == d2
来源：http://fxe.pycfn.com

[J08] 提取年月日与星期
来源：http://dmc.havefunace.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://imn.snrcjt.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qbx.yonumen.top


<!-- 参考信息 -->