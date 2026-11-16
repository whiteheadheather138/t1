代发 wailian999

[G10] 访问控制
来源：http://wuh.andypj.xyz

Py:   约定 _protected / __private（不强制）
来源：http://sww.svipenyu.cn

PHP:  public / protected / private
来源：http://doi.fktsv.cn

JS:   #private 字段；其余公开
来源：http://wnj.cucudq.cn

TS:   public / protected / private
来源：http://jyh.sxryk.cn

Java: public / protected / private / 默认包级
来源：http://bnf.cheryme.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://yzs.cashguo.top

Ruby: public / protected / private
来源：http://bvc.birdmap.top

C#:   public / protected / private / internal
来源：http://kqv.yonumen.top

[G11] getter / setter
来源：http://dkj.zhoulong.xyz

Py:   @property 与 @x.setter
来源：http://goh.ctjpmb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://vzu.wangdashe.top

JS:   get name() { return this._name; }
来源：http://req.jianghu66.top

TS:   get name(): string { return this._name; }
来源：http://aew.ctjpmb.com

Java: public String getName() { return name; }
来源：http://wqm.yvedp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hzc.tarul.cn

Ruby: attr_accessor :name
来源：http://tql.yj20258.top

C#:   public string Name { get; set; }
来源：http://erb.ivvv.top

[G12] 对象转字符串
来源：http://ejt.xuanzx.com

Py:   def __str__(self): return self.name
来源：http://bgf.shuidangran.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pou.jinyuanbaomall.cn

JS:   toString() { return this.name; }
来源：http://oua.jqgfzy.top

TS:   toString(): string { return this.name; }
来源：http://cgl.bjfxy.top

Java: @Override public String toString() { return name; }
来源：http://vpk.pengpengdd.cyou

Go:   func (u User) String() string { return u.Name }
来源：http://umg.xylfe.cn

Ruby: def to_s; @name; end
来源：http://sas.yj20258888.top

C#:   public override string ToString() => Name;
来源：http://ljf.sxryk.cn

[G13] 判断对象类型
来源：http://nvw.yj202588.top

Py:   isinstance(u, User)
来源：http://isg.jqgfzy.top

PHP:  $u instanceof User
来源：http://boa.zhaomingkeji.xyz

JS:   u instanceof User
来源：http://zrx.cheryme.top

TS:   u instanceof User
来源：http://fpn.svipenyu.cn

Java: u instanceof User
来源：http://noo.fktsv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pqh.zhengqikj.top

Ruby: u.is_a?(User)
来源：http://umt.zhiwuduotai.top

C#:   u is User
来源：http://eiw.hnqzz.top

[G14] 数据类 / record
来源：http://bmn.cqqwz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kgc.smart0.xyz

PHP:  // 用 readonly 属性模拟
来源：http://sce.guannengcc.top

JS:   // 无内置：普通类或对象字面量
来源：http://mcw.smart0.xyz

TS:   type User = { name: string; age: number };
来源：http://bty.shangyingyoupin.top

Java: record User(String name, int age) {}
来源：http://uua.jqgfzy.top

Go:   type User struct { Name string; Age int }
来源：http://qki.yueranfly.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vin.jlsjyb.cn

C#:   record User(string Name, int Age);
来源：http://xln.jlsjyb.cn

[G15] 枚举
来源：http://ibg.xingfuxueyuan.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vjk.tian-w.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bni.pengpengdd.cyou

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gru.yfazqb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fxr.yueranfly.top

Java: enum Color { RED, GREEN }
来源：http://ecd.hcnkem.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yyy.aizwys.cn

Ruby: Color = %i[red green].freeze
来源：http://uqx.mhx1999.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cyl.haohaochexian.top

[G16] 对象转数组 / 字典
来源：http://szm.jyoumei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lsy.xylfe.cn

PHP:  get_object_vars($obj);
来源：http://mpq.xziqi.cn

JS:   Object.entries(obj)
来源：http://rqp.zhengqikj.top

TS:   Object.entries(obj)
来源：http://jad.nwbrower.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jbv.hcnkem.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://wsg.shanyushiyangkeji.top

Ruby: obj.instance_variables
来源：http://gbq.iojbl.cn

C#:   // 用反射或 System.Text.Json
来源：http://lgc.xuanzx.com

================================================================================
来源：http://xkw.52xcode.cn

H. 异常与错误处理
来源：http://rhc.yongpay.top

================================================================================
来源：http://tud.xuanzx.com

[H01] try / catch 基础
来源：http://sqg.wangdashe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dfw.zdqjudy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hid.jinyuanbaomall.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://drd.yvedp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hrc.ydzc1.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xzd.yueranfly.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://exk.tarul.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dsw.daria6918.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tzn.jinqigufen.top

[H02] finally / ensure 收尾
来源：http://acv.fanxiaobao.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://kvv.jqgfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fne.sxryk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tas.gzhubu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://kqp.jqgufenzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://ndu.sxryk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://whs.daria6918.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vte.cheryme.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://hgp.zhijiandao.cn

[H03] 主动抛出异常
来源：http://omy.guowangkeji.top

Py:   raise ValueError("错误信息")
来源：http://vlv.fktsv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kit.zhijiandao.cn

JS:   throw new Error("错误信息");
来源：http://tlj.ehwqpu.com

TS:   throw new Error("错误信息");
来源：http://olx.chenlongwang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kts.meibo888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gsu.birdmap.top

Ruby: raise ArgumentError, "错误信息"
来源：http://iaw.guannengcc.top

C#:   throw new ArgumentException("错误信息");
来源：http://ksd.xylfe.cn

[H04] 自定义异常类型
来源：http://fsu.wangdashe.top

Py:   class MyError(Exception): pass
来源：http://fpf.yuxming.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tqh.ivvv.top

JS:   class MyError extends Error {}
来源：http://mot.jinqigufen.top

TS:   class MyError extends Error {}
来源：http://gqa.yj202588.top

Java: class MyException extends RuntimeException {}
来源：http://qzo.yueranfly.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hev.yj20258.top

Ruby: class MyError < StandardError; end
来源：http://qih.birdmap.top

C#:   class MyException : Exception {}
来源：http://prn.chenjidiqi.icu

[H05] 捕获特定类型
来源：http://epo.zhongyouzk.top

Py:   except ValueError as e:
来源：http://jwh.svipenyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nwy.sjlbkw.cn

JS:   if (e instanceof TypeError) {}
来源：http://ixr.dashuyun.cn

TS:   if (e instanceof TypeError) {}
来源：http://tjn.nwbrower.top

Java: catch (IOException | SQLException e) {}
来源：http://pwe.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kxw.yongpay.top

Ruby: rescue ArgumentError => e
来源：http://uds.0kj1m.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lgt.ppjwa.cn

[H06] 可选值 / 空值安全访问
来源：http://elg.yj202588.top

Py:   value = d.get("k") or default
来源：http://zfp.cucudq.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mem.yj20258888.top

JS:   obj?.a?.b;  d ?? default
来源：http://rrr.yueranfly.top

TS:   obj?.a?.b;  d ?? default
来源：http://ahl.316326.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tky.jqgufenzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://imq.chenzaomai.com

Ruby: d&.dig(:a, :b)
来源：http://bve.shuidangran.top

C#:   obj?.A?.B ?? default
来源：http://vlv.redwolf501.top

[H07] 断言
来源：http://yhi.hnxiangtu.top

Py:   assert x > 0, "必须为正"
来源：http://get.zhengqikj.top

PHP:  assert($x > 0);
来源：http://waf.jlsjyb.cn

JS:   console.assert(x > 0);
来源：http://adl.xziqi.cn

TS:   console.assert(x > 0);
来源：http://jlt.chenjidiqi.icu

Java: assert x > 0 : "必须为正";
来源：http://yyq.gaohongyu789.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xdr.quarkkingdee.top

Ruby: raise "必须为正" unless x > 0
来源：http://ezq.0kj1m.cn

C#:   Debug.Assert(x > 0);
来源：http://nad.fehbvm.com

[H08] 获取错误信息与堆栈
来源：http://znc.fehbvm.com

Py:   str(e);  traceback.format_exc()
来源：http://rtf.zhaomingkeji.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bfg.fzhhl.top

JS:   e.message;  e.stack
来源：http://hik.jinyuanbaomall.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sly.hfpthk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ddq.quarkkingdee.top

Go:   err.Error()
来源：http://fps.yvedp.cn

Ruby: e.message;  e.backtrace
来源：http://cdx.0kj1m.cn

C#:   e.Message;  e.StackTrace
来源：http://hha.zhongyouzk.top

[H09] 带错误码的异常
来源：http://ibo.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tqq.quarkkingdee.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qwb.fehbvm.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xvh.chenzaomai.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://idl.0kj1m.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ffr.shanyushiyangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yzj.hongshengwenyu.top

Ruby: raise MyError.new("fail", 500)
来源：http://qwo.nanxinkj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://hro.xylfe.cn

[H10] 资源自动释放
来源：http://umf.pengpengdd.cyou

Py:   with open("a.txt") as f: data = f.read()
来源：http://swi.ehwqpu.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bkg.andypj.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://chw.jqgfzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://azs.hfpthk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tjb.52xcode.cn

Go:   defer f.Close()
来源：http://kre.fzhhl.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://doe.tanke756.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fmw.zhengqikj.top

================================================================================
来源：http://epx.wangdashe.top

I. 正则表达式
来源：http://gbi.fanxiaobao.xyz

================================================================================
来源：http://cbt.hywenlv.cn

[I01] 判断是否匹配
来源：http://gkx.havefunace.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://azo.yueranfly.top

PHP:  preg_match('/\d+/', $s);
来源：http://xce.daria6918.cn

JS:   /\d+/.test(s)
来源：http://ept.iojbl.cn

TS:   /\d+/.test(s)
来源：http://apk.sweek.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ejv.52xcode.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ncm.gaohongyu789.top

Ruby: s.match?(/\d+/)
来源：http://kdr.52xcode.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dor.hammf.cn

[I02] 提取所有匹配
来源：http://wck.zhengqikj.top

Py:   re.findall(r"\d+", s)
来源：http://iix.epnwcf.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lmu.zhengqikj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jlq.pycfn.com

TS:   s.match(/\d+/g)
来源：http://nfj.zhengqikj.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://png.birdmap.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mza.shzxlz.cn

Ruby: s.scan(/\d+/)
来源：http://cfw.uphjek.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://aas.zdqjudy.top

[I03] 提取捕获分组
来源：http://mnt.jlsjyb.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aks.wangshuangyany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zls.jiagoushi.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hju.xinyue.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pnr.shzxlz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kqd.haohaochexian.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://via.jinqigufen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gug.pengpengdd.cyou

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://alb.meibo888.top

[I04] 正则替换
来源：http://odn.gaohongyu789.top

Py:   re.sub(r"\d+", "#", s)
来源：http://shc.bbcook.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hlx.shangyingyoupin.top

JS:   s.replace(/\d+/g, "#")
来源：http://yge.fanxiaobao.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://pum.yangfankeji.com

Java: s.replaceAll("\\d+", "#")
来源：http://kad.svipenyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ixe.0kj1m.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vym.9152youxi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mok.daxiang520.top

[I05] 按正则拆分
来源：http://epb.sxryk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yyx.zhijiandao.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fun.nanxinkj.top

JS:   s.split(/\s*,\s*/)
来源：http://zlz.ybcxt.top

TS:   s.split(/\s*,\s*/)
来源：http://btu.aibaodan.cn

Java: s.split("\\s*,\\s*")
来源：http://yrw.ivvv.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://coo.ppjwa.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nll.jinghuilouyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://afe.ehwqpu.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://scw.xuanzx.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://elb.yuanzhike.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ekd.sufxvd.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rsk.zhaomingkeji.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://srb.hfpthk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://imb.hnxiangtu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ciq.tianlin.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://flk.meibo888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qur.hnxiangtu.top

[I07] 忽略大小写与多行模式
来源：http://bmv.fanxiaobao.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ejk.zhixingplan.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iqv.smart0.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://afh.aizwys.cn

TS:   /error/gim
来源：http://feq.jiagoushi.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://agw.hcnkem.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nte.smart0.xyz

Ruby: s.scan(/error/i)
来源：http://rsb.jlsjyb.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tsj.redwolf501.top

[I08] 贪婪与非贪婪匹配
来源：http://gjv.yj202588.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gxt.yonumen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://moz.quarkkingdee.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fyf.chenjidiqi.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iqc.pycfn.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://soh.cqqwz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ghv.uphjek.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://asa.pengpengdd.cyou

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ewd.sjlbkw.cn

================================================================================
来源：http://skk.ctjpmb.com

J. 日期与时间
来源：http://btm.jqgufenzy.top

================================================================================
来源：http://lff.ehwqpu.com

[J01] 获取当前时间
来源：http://trd.bbcook.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zya.haohaochexian.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zrr.redwolf501.top

JS:   new Date();  Date.now()
来源：http://nqm.yj202588.top

TS:   new Date();  Date.now()
来源：http://izb.yj202588.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qod.jinqigfzy.top

Go:   time.Now()
来源：http://odj.ctjpmb.com

Ruby: Time.now
来源：http://tue.vehdjk.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zfw.chenzaomai.com

[J02] 格式化输出
来源：http://urh.fktsv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wyg.ehwqpu.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nte.xziqi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xxx.sufxvd.cn

TS:   d.toISOString()
来源：http://txm.zdqjudy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yuz.jiagoushi.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://iqd.cucudq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yhk.epnwcf.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://soc.zycfv.cn

[J03] 字符串解析为日期
来源：http://sar.quarkkingdee.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cwk.nanxuanxn.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://krh.guowangkeji.top

JS:   new Date("2024-01-02")
来源：http://hcn.chenjidiqi.icu

TS:   new Date("2024-01-02")
来源：http://bgx.hfpthk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pwb.pycfn.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fsz.hammf.cn

Ruby: Date.parse("2024-01-02")
来源：http://mvt.xinyue.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ywa.fanxiaobao.xyz

[J04] 时间戳与日期互转
来源：http://deo.wangdashe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://owt.gogol.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jxu.fzhhl.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ejr.sweek.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zfi.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://trr.fengsongda.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://okp.xuanzx.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zsa.aibaodan.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ygy.zhixingplan.top

[J05] 时间加减（加 7 天）
来源：http://xmj.fehbvm.com

Py:   now + timedelta(days=7)
来源：http://vip.epnwcf.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://zul.jianghu66.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yby.0kj1m.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dii.bbcook.cn

Java: LocalDate.now().plusDays(7)
来源：http://aqo.bjfxy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sbd.hesvh.cn

Ruby: Time.now + 7 * 86400
来源：http://vbe.yongpay.top

C#:   DateTime.Now.AddDays(7)
来源：http://mpg.sysykeji.top

[J06] 计算两时间之差
来源：http://wam.daria6918.cn

Py:   (end - start).total_seconds()
来源：http://ite.9152youxi.cn

PHP:  $end->diff($start)->days;
来源：http://cls.fehbvm.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://roy.sjlbkw.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zwj.52xcode.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wqm.yonumen.top

Go:   end.Sub(start).Hours()
来源：http://fug.hnqzz.top

Ruby: end - start                 # 返回秒数
来源：http://wlp.feifeiyinyue.top

C#:   (end - start).TotalSeconds
来源：http://efm.tianlin.xyz

[J07] 比较两个日期
来源：http://lez.yj202588.top

Py:   d1 < d2;  d1 == d2
来源：http://bbf.hywenlv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sfs.yanxiufei.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xet.shanyushiyangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://wwr.cheryme.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nrs.ppjwa.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bvw.shuidangran.top

Ruby: d1 < d2;  d1 == d2
来源：http://xku.yuanzhike.top

C#:   d1 < d2;  d1 == d2
来源：http://kfr.gzhubu.top

[J08] 提取年月日与星期
来源：http://ezj.xuetiantiany.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jom.snrcjt.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xpz.ydjk.org.cn


<!-- 参考信息 -->