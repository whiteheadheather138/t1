代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://rqf.ivvv.top

Ruby: def self.f; end
来源：http://ttw.cqqwz.cn

C#:   public static void F() {}
来源：http://alt.yfazqb.com

[G09] 接口 / 抽象类
来源：http://bbe.xingfuxueyuan.xyz

Py:   from abc import ABC, abstractmethod
来源：http://gme.yueranfly.top

PHP:  interface Shape { public function area(): float; }
来源：http://qys.ivvv.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zcp.xinyue.icu

TS:   interface Shape { area(): number; }
来源：http://gyf.fktsv.cn

Java: interface Shape { double area(); }
来源：http://apr.zdqjudy.top

Go:   type Shape interface { Area() float64 }
来源：http://kul.bbcook.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://aar.nanxinkj.top

C#:   interface IShape { double Area(); }
来源：http://iuq.jyoumei.cn

[G10] 访问控制
来源：http://ofj.kuanghao11.cn

Py:   约定 _protected / __private（不强制）
来源：http://rsv.nanxinkj.top

PHP:  public / protected / private
来源：http://iak.kuanghao11.cn

JS:   #private 字段；其余公开
来源：http://dto.birdmap.top

TS:   public / protected / private
来源：http://bmm.xingfuxueyuan.xyz

Java: public / protected / private / 默认包级
来源：http://wuj.0kj1m.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://owh.shzxlz.cn

Ruby: public / protected / private
来源：http://anv.316326.xyz

C#:   public / protected / private / internal
来源：http://uyh.tian-w.cn

[G11] getter / setter
来源：http://uox.chenzaomai.com

Py:   @property 与 @x.setter
来源：http://wmb.vqdsnc.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hii.gaohongyu789.top

JS:   get name() { return this._name; }
来源：http://qvj.cqqwz.cn

TS:   get name(): string { return this._name; }
来源：http://zjt.cheryme.top

Java: public String getName() { return name; }
来源：http://qyq.fzhhl.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://egc.ybcxt.top

Ruby: attr_accessor :name
来源：http://ffk.cashguo.top

C#:   public string Name { get; set; }
来源：http://ysw.ydzc1.top

[G12] 对象转字符串
来源：http://tan.fengsongda.top

Py:   def __str__(self): return self.name
来源：http://gta.pengpengdd.cyou

PHP:  public function __toString(): string { return $this->name; }
来源：http://wzn.ehwqpu.com

JS:   toString() { return this.name; }
来源：http://pus.haohaochexian.top

TS:   toString(): string { return this.name; }
来源：http://zwj.pengpengdd.cyou

Java: @Override public String toString() { return name; }
来源：http://yau.chenzaomai.com

Go:   func (u User) String() string { return u.Name }
来源：http://snv.jinyuanbaomall.cn

Ruby: def to_s; @name; end
来源：http://usv.jinyuanbaomall.cn

C#:   public override string ToString() => Name;
来源：http://mks.andypj.xyz

[G13] 判断对象类型
来源：http://tmf.fanxiaobao.xyz

Py:   isinstance(u, User)
来源：http://chz.jqgfzy.top

PHP:  $u instanceof User
来源：http://uxb.hnqzz.top

JS:   u instanceof User
来源：http://mhr.vehdjk.com

TS:   u instanceof User
来源：http://apf.316326.xyz

Java: u instanceof User
来源：http://bto.yuxming.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nuo.chenjidiqi.icu

Ruby: u.is_a?(User)
来源：http://nhb.kuanghao11.cn

C#:   u is User
来源：http://udz.yonumen.top

[G14] 数据类 / record
来源：http://lwj.aizwys.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hae.ctjpmb.com

PHP:  // 用 readonly 属性模拟
来源：http://zhj.yvedp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jea.ppjwa.cn

TS:   type User = { name: string; age: number };
来源：http://eme.jlsjyb.cn

Java: record User(String name, int age) {}
来源：http://pla.vqdsnc.cn

Go:   type User struct { Name string; Age int }
来源：http://jpu.andypj.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ktt.fengsongda.top

C#:   record User(string Name, int Age);
来源：http://qqt.fengsongda.top

[G15] 枚举
来源：http://lgy.tian-w.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uub.nwbrower.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ujq.0kj1m.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ecu.ybcxt.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vdd.chenzaomai.com

Java: enum Color { RED, GREEN }
来源：http://znh.xylfe.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://khy.jinqigfzy.top

Ruby: Color = %i[red green].freeze
来源：http://rit.jqgfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://edi.svipenyu.cn

[G16] 对象转数组 / 字典
来源：http://dts.ehwqpu.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://plh.epnwcf.com

PHP:  get_object_vars($obj);
来源：http://qak.xziqi.cn

JS:   Object.entries(obj)
来源：http://ofd.snrcjt.cn

TS:   Object.entries(obj)
来源：http://oyu.iojbl.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rii.zhongyouzk.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vcy.cqqwz.cn

Ruby: obj.instance_variables
来源：http://jaw.wangdashe.top

C#:   // 用反射或 System.Text.Json
来源：http://xnc.hfpthk.cn

================================================================================
来源：http://frj.yj202588.top

H. 异常与错误处理
来源：http://ydd.zhiwuduotai.top

================================================================================
来源：http://goo.gzhubu.top

[H01] try / catch 基础
来源：http://qie.xziqi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://aws.cashguo.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cmq.xinyue.icu

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tpp.tarul.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wno.fanxiaobao.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wsx.andypj.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jwg.yanxiufei.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pho.ydzc1.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://onf.dianchejie.cn

[H02] finally / ensure 收尾
来源：http://ltp.iojbl.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jng.9152youxi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xwe.jinqigufen.top

JS:   try { f(); } finally { cleanup(); }
来源：http://com.ybcxt.top

TS:   try { f(); } finally { cleanup(); }
来源：http://eng.guowangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://amx.nanxuanxn.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mxn.mhx1999.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vge.jyoumei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pps.daria6918.cn

[H03] 主动抛出异常
来源：http://ubk.kuanghao11.cn

Py:   raise ValueError("错误信息")
来源：http://tsd.zycfv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://njq.iojbl.cn

JS:   throw new Error("错误信息");
来源：http://jam.hcnkem.com

TS:   throw new Error("错误信息");
来源：http://aec.zhoulong.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://kff.9152youxi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jzc.shanyushiyangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hmr.pycfn.com

C#:   throw new ArgumentException("错误信息");
来源：http://ojc.tarul.cn

[H04] 自定义异常类型
来源：http://cgc.cqqwz.cn

Py:   class MyError(Exception): pass
来源：http://fuv.quarkkingdee.top

PHP:  class MyError extends RuntimeException {}
来源：http://bgm.iojbl.cn

JS:   class MyError extends Error {}
来源：http://ltq.tanke756.top

TS:   class MyError extends Error {}
来源：http://nta.yj20258.top

Java: class MyException extends RuntimeException {}
来源：http://zfj.jinyuanbaomall.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://elo.jqgufenzy.top

Ruby: class MyError < StandardError; end
来源：http://bro.zhiwuduotai.top

C#:   class MyException : Exception {}
来源：http://yls.yuanzhike.top

[H05] 捕获特定类型
来源：http://xoc.yvedp.cn

Py:   except ValueError as e:
来源：http://nlm.svipenyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mnl.uphjek.com

JS:   if (e instanceof TypeError) {}
来源：http://dwa.c1oappe.top

TS:   if (e instanceof TypeError) {}
来源：http://pzr.birdmap.top

Java: catch (IOException | SQLException e) {}
来源：http://rqe.jqgufenzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vpq.wangshuangyany.cn

Ruby: rescue ArgumentError => e
来源：http://njj.wangshuangyany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://itw.fengsongda.top

[H06] 可选值 / 空值安全访问
来源：http://zrv.ydzc1.top

Py:   value = d.get("k") or default
来源：http://vuq.aizwys.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jit.bjfxy.top

JS:   obj?.a?.b;  d ?? default
来源：http://hpq.birdmap.top

TS:   obj?.a?.b;  d ?? default
来源：http://qwm.chenzaomai.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://olw.andypj.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://cki.fktsv.cn

Ruby: d&.dig(:a, :b)
来源：http://jwz.316326.xyz

C#:   obj?.A?.B ?? default
来源：http://osp.wangdashe.top

[H07] 断言
来源：http://osx.chenlongwang.top

Py:   assert x > 0, "必须为正"
来源：http://eav.ydzc1.top

PHP:  assert($x > 0);
来源：http://kcd.sjlbkw.cn

JS:   console.assert(x > 0);
来源：http://gyu.cdnleiting.top

TS:   console.assert(x > 0);
来源：http://jsk.xuetiantiany.cn

Java: assert x > 0 : "必须为正";
来源：http://zrx.cashguo.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xnt.jinyuanbaomall.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ygw.guannengcc.top

C#:   Debug.Assert(x > 0);
来源：http://ylj.tanke756.top

[H08] 获取错误信息与堆栈
来源：http://isu.zhongyouzk.top

Py:   str(e);  traceback.format_exc()
来源：http://osq.jinqigufen.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tiv.guannengcc.top

JS:   e.message;  e.stack
来源：http://agw.yongpay.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fqo.yongpay.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ent.yfazqb.com

Go:   err.Error()
来源：http://gyp.bjfxy.top

Ruby: e.message;  e.backtrace
来源：http://ysb.hesvh.cn

C#:   e.Message;  e.StackTrace
来源：http://uhi.shuidangran.top

[H09] 带错误码的异常
来源：http://xej.shuidangran.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ckc.zdqjudy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mvv.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nph.dianchejie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bnb.fanxiaobao.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wcz.52xcode.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bxa.feifeiyinyue.top

Ruby: raise MyError.new("fail", 500)
来源：http://koa.aizwys.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vip.ydjk.org.cn

[H10] 资源自动释放
来源：http://lks.zhiwuduotai.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://uqa.shanyushiyangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://urn.c1oappe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zek.hfpthk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://obz.zycfv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xwe.shangyingyoupin.top

Go:   defer f.Close()
来源：http://fbd.fzhhl.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hke.ybcxt.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tsv.nanxuanxn.top

================================================================================
来源：http://itt.ybcxt.top

I. 正则表达式
来源：http://ipx.zhixingplan.top

================================================================================
来源：http://nqi.gaohongyu789.top

[I01] 判断是否匹配
来源：http://cch.nwbrower.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vej.aizwys.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qta.0kj1m.cn

JS:   /\d+/.test(s)
来源：http://ulz.fehbvm.com

TS:   /\d+/.test(s)
来源：http://jrs.meibo888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ugf.aizwys.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uue.ydzc1.top

Ruby: s.match?(/\d+/)
来源：http://csw.redwolf501.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nxj.dianchejie.cn

[I02] 提取所有匹配
来源：http://zrw.jiagoushi.top

Py:   re.findall(r"\d+", s)
来源：http://wub.hammf.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kwn.fehbvm.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zyz.guowangkeji.top

TS:   s.match(/\d+/g)
来源：http://hxk.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mzj.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mvs.chenjidiqi.icu

Ruby: s.scan(/\d+/)
来源：http://sqq.zdbjq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tpa.9152youxi.cn

[I03] 提取捕获分组
来源：http://szv.fzhhl.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lgc.xuanzx.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jvy.zhaomingkeji.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vpn.jinqigufen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zip.meibo888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xci.gogol.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zvs.zhongyouzk.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vfp.hesvh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yge.fanxiaobao.xyz

[I04] 正则替换
来源：http://bmv.wangshuangyany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tpg.ywan-chungtsiang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://drn.nwbrower.top

JS:   s.replace(/\d+/g, "#")
来源：http://waq.ppjwa.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bji.meibo888.top

Java: s.replaceAll("\\d+", "#")
来源：http://rpb.shanyushiyangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://owt.jqgfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://puc.havefunace.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://evg.guowangkeji.top

[I05] 按正则拆分
来源：http://cwu.jyoumei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://etj.jinqigfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uem.jiagoushi.top

JS:   s.split(/\s*,\s*/)
来源：http://noe.wangshuangyany.cn

TS:   s.split(/\s*,\s*/)
来源：http://clo.yj20258.top

Java: s.split("\\s*,\\s*")
来源：http://ihk.fzhhl.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jrr.uphjek.com

Ruby: s.split(/\s*,\s*/)
来源：http://gna.vqdsnc.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lcm.sxryk.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://loi.bjfxy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pss.zhengqikj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pgx.yanxiufei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ajl.hammf.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://thh.yuanzhike.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jrw.fanxiaobao.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xtw.ivvv.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hlf.nwbrower.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://syu.tarul.cn

[I07] 忽略大小写与多行模式
来源：http://yoo.jinyuanbaomall.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qhj.ehwqpu.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qla.316326.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nkz.cucudq.cn

TS:   /error/gim
来源：http://rsr.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://aej.vqdsnc.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jsw.xziqi.cn

Ruby: s.scan(/error/i)
来源：http://nfe.chenzaomai.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zaq.316326.xyz

[I08] 贪婪与非贪婪匹配
来源：http://rbc.feifeiyinyue.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lsr.yangfankeji.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yuh.daxiang520.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xum.cheryme.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://erx.zdqjudy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://aga.snrcjt.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ryc.vehdjk.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://asy.gogol.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uwp.shanyushiyangkeji.top

================================================================================
来源：http://wwp.shzxlz.cn

J. 日期与时间
来源：http://agy.shuidangran.top

================================================================================
来源：http://vdb.yanxiufei.cn

[J01] 获取当前时间
来源：http://mat.iojbl.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vds.havefunace.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zdp.tianlin.xyz

JS:   new Date();  Date.now()
来源：http://mgy.xinyue.icu

TS:   new Date();  Date.now()
来源：http://uiz.hnqzz.top

Java: LocalDateTime.now();  Instant.now()
来源：http://hxu.xingfuxueyuan.xyz

Go:   time.Now()
来源：http://olk.zhijiandao.cn

Ruby: Time.now
来源：http://zqg.316326.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vra.wangdashe.top

[J02] 格式化输出
来源：http://yli.hywenlv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://naq.daxiang520.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sty.dianchejie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hxu.zdbjq.cn

TS:   d.toISOString()
来源：http://ucc.yj202588.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://boq.daxiang520.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zad.hnqzz.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uyh.shzxlz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://daz.yongpay.top

[J03] 字符串解析为日期
来源：http://hmb.aibaodan.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cha.hysaishi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uko.xziqi.cn

JS:   new Date("2024-01-02")
来源：http://bts.52xcode.cn

TS:   new Date("2024-01-02")
来源：http://cbv.guannengcc.top

Java: LocalDate.parse("2024-01-02")
来源：http://pnp.hywenlv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sfd.xylfe.cn

Ruby: Date.parse("2024-01-02")
来源：http://wpu.pycfn.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vcs.gotoacloud.top

[J04] 时间戳与日期互转
来源：http://xaq.hnxiangtu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ats.52xcode.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://aig.svipenyu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lkx.jianghu66.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ixn.nanxuanxn.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rrx.cdnleiting.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jls.dashuyun.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mql.sysykeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cfa.sweek.top

[J05] 时间加减（加 7 天）
来源：http://mly.vehdjk.com

Py:   now + timedelta(days=7)
来源：http://eqx.hammf.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wfa.cdnleiting.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gbb.hnqzz.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pgb.yfazqb.com

Java: LocalDate.now().plusDays(7)
来源：http://ynn.vqdsnc.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oko.vqdsnc.cn

Ruby: Time.now + 7 * 86400
来源：http://jvu.meibo888.top

C#:   DateTime.Now.AddDays(7)
来源：http://vmr.yueranfly.top

[J06] 计算两时间之差
来源：http://row.ydzc1.top

Py:   (end - start).total_seconds()
来源：http://gnh.dashuyun.cn

PHP:  $end->diff($start)->days;
来源：http://vlx.daxiang520.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://okk.c1oappe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xto.tarul.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nne.yonumen.top

Go:   end.Sub(start).Hours()
来源：http://gmp.yuanzhike.top

Ruby: end - start                 # 返回秒数
来源：http://nde.fehbvm.com

C#:   (end - start).TotalSeconds
来源：http://csd.jinyuanbaomall.cn


<!-- 参考信息 -->