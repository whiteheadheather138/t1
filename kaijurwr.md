代发 wailian999

Java: interface Shape { double area(); }
来源：http://hwl.cashguo.top

Go:   type Shape interface { Area() float64 }
来源：http://shq.hnxiangtu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ypg.iojbl.cn

C#:   interface IShape { double Area(); }
来源：http://dux.sjlbkw.cn

[G10] 访问控制
来源：http://cin.shzxlz.cn

Py:   约定 _protected / __private（不强制）
来源：http://noa.andypj.xyz

PHP:  public / protected / private
来源：http://aac.chenlongwang.top

JS:   #private 字段；其余公开
来源：http://jqk.zhongyouzk.top

TS:   public / protected / private
来源：http://mqo.jqgufenzy.top

Java: public / protected / private / 默认包级
来源：http://uay.hfpthk.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://auh.bjfxy.top

Ruby: public / protected / private
来源：http://ibn.yj202588.top

C#:   public / protected / private / internal
来源：http://gki.ctjpmb.com

[G11] getter / setter
来源：http://ixt.aibaodan.cn

Py:   @property 与 @x.setter
来源：http://lqy.shzxlz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qrn.fengsongda.top

JS:   get name() { return this._name; }
来源：http://tob.ctjpmb.com

TS:   get name(): string { return this._name; }
来源：http://qkt.xylfe.cn

Java: public String getName() { return name; }
来源：http://jjv.fanxiaobao.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://xgw.zdqjudy.top

Ruby: attr_accessor :name
来源：http://vkg.jiagoushi.top

C#:   public string Name { get; set; }
来源：http://qss.zhiwuduotai.top

[G12] 对象转字符串
来源：http://wlz.0kj1m.cn

Py:   def __str__(self): return self.name
来源：http://nax.feifeiyinyue.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qqu.zhixingplan.top

JS:   toString() { return this.name; }
来源：http://ymk.mhx1999.top

TS:   toString(): string { return this.name; }
来源：http://gus.gaohongyu789.top

Java: @Override public String toString() { return name; }
来源：http://nfx.tanke756.top

Go:   func (u User) String() string { return u.Name }
来源：http://jtg.dianchejie.cn

Ruby: def to_s; @name; end
来源：http://tyv.daxiang520.top

C#:   public override string ToString() => Name;
来源：http://loi.bjfxy.top

[G13] 判断对象类型
来源：http://mxr.yj20258.top

Py:   isinstance(u, User)
来源：http://zxu.gogol.net.cn

PHP:  $u instanceof User
来源：http://dqw.redwolf501.top

JS:   u instanceof User
来源：http://wlk.jlsjyb.cn

TS:   u instanceof User
来源：http://fmi.xinyue.icu

Java: u instanceof User
来源：http://dyl.haohaochexian.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://rjf.cqqwz.cn

Ruby: u.is_a?(User)
来源：http://dft.tianlin.xyz

C#:   u is User
来源：http://ekn.sjlbkw.cn

[G14] 数据类 / record
来源：http://fos.andypj.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ftv.jqgufenzy.top

PHP:  // 用 readonly 属性模拟
来源：http://jvy.bbcook.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cco.sufxvd.cn

TS:   type User = { name: string; age: number };
来源：http://eeg.andypj.xyz

Java: record User(String name, int age) {}
来源：http://uig.aizwys.cn

Go:   type User struct { Name string; Age int }
来源：http://fcv.kuanghao11.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jnb.redwolf501.top

C#:   record User(string Name, int Age);
来源：http://rik.hywenlv.cn

[G15] 枚举
来源：http://mgj.uphjek.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://iha.yanxiufei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fzm.wangshuangyany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xkf.epnwcf.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gho.daxiang520.top

Java: enum Color { RED, GREEN }
来源：http://czb.yanxiufei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fbz.yuxming.cn

Ruby: Color = %i[red green].freeze
来源：http://otd.jqgfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rur.hesvh.cn

[G16] 对象转数组 / 字典
来源：http://edn.vqdsnc.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rvk.hnxiangtu.top

PHP:  get_object_vars($obj);
来源：http://ycd.cqqwz.cn

JS:   Object.entries(obj)
来源：http://iij.0kj1m.cn

TS:   Object.entries(obj)
来源：http://kcf.daria6918.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://euw.tian-w.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jjm.bjfxy.top

Ruby: obj.instance_variables
来源：http://xhq.ybcxt.top

C#:   // 用反射或 System.Text.Json
来源：http://ddi.9152youxi.cn

================================================================================
来源：http://kcq.redwolf501.top

H. 异常与错误处理
来源：http://xbd.epnwcf.com

================================================================================
来源：http://xke.jinqigfzy.top

[H01] try / catch 基础
来源：http://ako.tarul.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dyy.nanxinkj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ain.hysaishi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vof.zhijiandao.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vjc.sxryk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mfl.jinqigufen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://psb.shzxlz.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bpz.uphjek.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tye.pycfn.com

[H02] finally / ensure 收尾
来源：http://uxn.fanxiaobao.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://uml.yvedp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wkk.iojbl.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kxz.hesvh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zuh.shanyushiyangtech.top

Java: try { f(); } finally { cleanup(); }
来源：http://mzi.9152youxi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jnd.fzhhl.top

Ruby: begin; f; ensure; cleanup; end
来源：http://olf.guowangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xqk.chenlongwang.top

[H03] 主动抛出异常
来源：http://elp.wangshuangyany.cn

Py:   raise ValueError("错误信息")
来源：http://zwu.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://haq.zdbjq.cn

JS:   throw new Error("错误信息");
来源：http://yqk.wangshuangyany.cn

TS:   throw new Error("错误信息");
来源：http://tmg.sxryk.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lku.gaohongyu789.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yhs.smart0.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://xrb.yangfankeji.com

C#:   throw new ArgumentException("错误信息");
来源：http://umi.jqgufenzy.top

[H04] 自定义异常类型
来源：http://nux.jinghuilouyu.cn

Py:   class MyError(Exception): pass
来源：http://hlg.sweek.top

PHP:  class MyError extends RuntimeException {}
来源：http://vqb.vqdsnc.cn

JS:   class MyError extends Error {}
来源：http://hwp.chenlongwang.top

TS:   class MyError extends Error {}
来源：http://cqd.sufxvd.cn

Java: class MyException extends RuntimeException {}
来源：http://tll.ydjk.org.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://evd.hywenlv.cn

Ruby: class MyError < StandardError; end
来源：http://rjy.xylfe.cn

C#:   class MyException : Exception {}
来源：http://iyv.bjfxy.top

[H05] 捕获特定类型
来源：http://ucs.yfazqb.com

Py:   except ValueError as e:
来源：http://kpc.ydzc1.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jce.wangdashe.top

JS:   if (e instanceof TypeError) {}
来源：http://yba.jianghu66.top

TS:   if (e instanceof TypeError) {}
来源：http://doa.gotoacloud.top

Java: catch (IOException | SQLException e) {}
来源：http://ihr.jianghu66.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://prr.jianghu66.top

Ruby: rescue ArgumentError => e
来源：http://lsm.yj20258.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vdk.zdqjudy.top

[H06] 可选值 / 空值安全访问
来源：http://zmx.guowangkeji.top

Py:   value = d.get("k") or default
来源：http://fsk.cdnleiting.top

PHP:  $v = $d["k"] ?? null;
来源：http://vyr.xylfe.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mlv.shanyushiyangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://grs.zhengqikj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mzj.xingfuxueyuan.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://tec.sufxvd.cn

Ruby: d&.dig(:a, :b)
来源：http://aus.feifeiyinyue.top

C#:   obj?.A?.B ?? default
来源：http://nme.cucudq.cn

[H07] 断言
来源：http://qzl.zycfv.cn

Py:   assert x > 0, "必须为正"
来源：http://qqc.meibo888.top

PHP:  assert($x > 0);
来源：http://brx.ppjwa.cn

JS:   console.assert(x > 0);
来源：http://erp.wangshuangyany.cn

TS:   console.assert(x > 0);
来源：http://kjl.ywan-chungtsiang.top

Java: assert x > 0 : "必须为正";
来源：http://uij.smart0.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kip.cashguo.top

Ruby: raise "必须为正" unless x > 0
来源：http://ijn.shanyushiyangtech.top

C#:   Debug.Assert(x > 0);
来源：http://tgs.pengpengdd.cyou

[H08] 获取错误信息与堆栈
来源：http://gig.haohaochexian.top

Py:   str(e);  traceback.format_exc()
来源：http://cic.guannengcc.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ebv.hongshengwenyu.top

JS:   e.message;  e.stack
来源：http://wyl.nanxinkj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ppd.xuetiantiany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cuz.dashuyun.cn

Go:   err.Error()
来源：http://xcv.gzhubu.top

Ruby: e.message;  e.backtrace
来源：http://nit.xuetiantiany.cn

C#:   e.Message;  e.StackTrace
来源：http://hzk.quarkkingdee.top

[H09] 带错误码的异常
来源：http://pcv.jlsjyb.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://usp.nanxinkj.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://aoj.yongpay.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ocu.daria6918.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cem.yanxiufei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://oqu.ybcxt.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cbm.sufxvd.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vyr.yvedp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://eam.chenzaomai.com

[H10] 资源自动释放
来源：http://oba.zhaomingkeji.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://jcd.chenlongwang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fzi.xziqi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ihq.yfazqb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qui.yj202588.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rmo.xingfuxueyuan.xyz

Go:   defer f.Close()
来源：http://muo.zycfv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lzr.hfpthk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tvs.aizwys.cn

================================================================================
来源：http://ljh.sjlbkw.cn

I. 正则表达式
来源：http://nkp.jianghu66.top

================================================================================
来源：http://shp.xinyue.icu

[I01] 判断是否匹配
来源：http://nse.wangdashe.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jap.shanyushiyangtech.top

PHP:  preg_match('/\d+/', $s);
来源：http://gxl.mhx1999.top

JS:   /\d+/.test(s)
来源：http://blf.tianlin.xyz

TS:   /\d+/.test(s)
来源：http://umw.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sjq.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rmp.fanxiaobao.xyz

Ruby: s.match?(/\d+/)
来源：http://lgd.fehbvm.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sfz.ppjwa.cn

[I02] 提取所有匹配
来源：http://hbf.xuanzx.com

Py:   re.findall(r"\d+", s)
来源：http://yit.bbcook.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yii.shuidangran.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://geh.gzhubu.top

TS:   s.match(/\d+/g)
来源：http://hdx.tianlin.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://emv.aizwys.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cwp.vehdjk.com

Ruby: s.scan(/\d+/)
来源：http://oqd.birdmap.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tya.birdmap.top

[I03] 提取捕获分组
来源：http://wjv.yj202588.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://his.fzhhl.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fxm.jianghu66.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gzt.cdnleiting.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nir.guowangkeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oks.zhoulong.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://auv.yueranfly.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vcc.smart0.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oky.birdmap.top

[I04] 正则替换
来源：http://zxm.cheryme.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jct.jinqigfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fnu.yuanzhike.top

JS:   s.replace(/\d+/g, "#")
来源：http://hpc.zdbjq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fwi.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://pyt.xuetiantiany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jag.hnxiangtu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://gpn.uphjek.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jjb.sysykeji.top

[I05] 按正则拆分
来源：http://tyj.fehbvm.com

Py:   re.split(r"\s*,\s*", s)
来源：http://lfv.fzhhl.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rtj.hysaishi.cn

JS:   s.split(/\s*,\s*/)
来源：http://rwv.snrcjt.cn

TS:   s.split(/\s*,\s*/)
来源：http://qwr.cucudq.cn

Java: s.split("\\s*,\\s*")
来源：http://fby.zhoulong.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ydn.bbcook.cn

Ruby: s.split(/\s*,\s*/)
来源：http://loq.tarul.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pqo.jqgufenzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://elx.cqqwz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iym.shanyushiyangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pre.mhx1999.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nlp.shanyushiyangtech.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ghd.gzhubu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hdq.hfpthk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mnq.feifeiyinyue.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fkh.wangshuangyany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ttw.iojbl.cn

[I07] 忽略大小写与多行模式
来源：http://bft.hnxiangtu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xyo.yj20258.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vkq.uphjek.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rbb.yj202588.top

TS:   /error/gim
来源：http://jlq.c1oappe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mxz.havefunace.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ijz.yj202588.top

Ruby: s.scan(/error/i)
来源：http://vxc.nanxuanxn.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ffn.jinqigufen.top

[I08] 贪婪与非贪婪匹配
来源：http://uor.jinqigfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://shf.bbcook.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uyz.daria6918.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dbp.fanxiaobao.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ywx.aizwys.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://grh.sysykeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jkx.yvedp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qph.daria6918.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wtu.svipenyu.cn

================================================================================
来源：http://zdi.sysykeji.top

J. 日期与时间
来源：http://egd.epnwcf.com

================================================================================
来源：http://duk.jinyuanbaomall.cn

[J01] 获取当前时间
来源：http://slg.yangfankeji.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://fzh.hongshengwenyu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://utc.yj20258.top

JS:   new Date();  Date.now()
来源：http://wuc.cashguo.top

TS:   new Date();  Date.now()
来源：http://egn.pengpengdd.cyou

Java: LocalDateTime.now();  Instant.now()
来源：http://ovu.fanxiaobao.xyz

Go:   time.Now()
来源：http://trj.nanxuanxn.top

Ruby: Time.now
来源：http://efn.cheryme.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ueo.uphjek.com

[J02] 格式化输出
来源：http://qzx.xinyue.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://idp.hcnkem.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jrs.jinqigfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://joh.shuidangran.top

TS:   d.toISOString()
来源：http://qjx.havefunace.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gpt.fktsv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kot.yonumen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://elq.ehwqpu.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nvd.snrcjt.cn

[J03] 字符串解析为日期
来源：http://cri.shuidangran.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fqi.sufxvd.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://izv.hesvh.cn

JS:   new Date("2024-01-02")
来源：http://vox.daria6918.cn

TS:   new Date("2024-01-02")
来源：http://gls.tian-w.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yar.yvedp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cry.yangfankeji.com

Ruby: Date.parse("2024-01-02")
来源：http://kzc.shanyushiyangtech.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kri.svipenyu.cn

[J04] 时间戳与日期互转
来源：http://wkj.chenlongwang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xgi.yj20258888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xve.sweek.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rsl.ydjk.org.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://frx.yonumen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gnu.gogol.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kzi.cucudq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://huy.birdmap.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nke.hfpthk.cn

[J05] 时间加减（加 7 天）
来源：http://znf.ivvv.top

Py:   now + timedelta(days=7)
来源：http://cuj.epnwcf.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://qlq.smart0.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jpj.tian-w.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://toz.zhoulong.xyz

Java: LocalDate.now().plusDays(7)
来源：http://zrm.ydzc1.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xug.shanyushiyangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://pbf.havefunace.top

C#:   DateTime.Now.AddDays(7)
来源：http://hdy.fanxiaobao.xyz

[J06] 计算两时间之差
来源：http://luu.shangyingyoupin.top

Py:   (end - start).total_seconds()
来源：http://jmf.svipenyu.cn

PHP:  $end->diff($start)->days;
来源：http://gke.wangdashe.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://usb.jqgufenzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xbm.zhijiandao.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xvv.xingfuxueyuan.xyz

Go:   end.Sub(start).Hours()
来源：http://ezb.svipenyu.cn

Ruby: end - start                 # 返回秒数
来源：http://hil.guannengcc.top

C#:   (end - start).TotalSeconds
来源：http://rdi.ppjwa.cn

[J07] 比较两个日期
来源：http://isb.jinqigfzy.top

Py:   d1 < d2;  d1 == d2
来源：http://jdj.aizwys.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ahk.hywenlv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://eon.redwolf501.top

TS:   d1.getTime() < d2.getTime()
来源：http://elc.hnqzz.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://smt.yuanzhike.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yub.tarul.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rrg.aizwys.cn


<!-- 参考信息 -->