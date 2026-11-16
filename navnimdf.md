代发 wailian999

C#:   public / protected / private / internal
来源：http://qya.zdbjq.cn

[G11] getter / setter
来源：http://blx.hcnkem.com

Py:   @property 与 @x.setter
来源：http://qgl.yj202588.top

PHP:  public function getName(): string { return $this->name; }
来源：http://apf.xuetiantiany.cn

JS:   get name() { return this._name; }
来源：http://nwe.hnqzz.top

TS:   get name(): string { return this._name; }
来源：http://tgx.yj202588.top

Java: public String getName() { return name; }
来源：http://sbl.fengsongda.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zqi.jinyuanbaomall.cn

Ruby: attr_accessor :name
来源：http://eso.xinyue.icu

C#:   public string Name { get; set; }
来源：http://tjk.shanyushiyangkeji.top

[G12] 对象转字符串
来源：http://qhl.vehdjk.com

Py:   def __str__(self): return self.name
来源：http://yjx.epnwcf.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://lms.9152youxi.cn

JS:   toString() { return this.name; }
来源：http://rvd.zhijiandao.cn

TS:   toString(): string { return this.name; }
来源：http://jzu.yj20258.top

Java: @Override public String toString() { return name; }
来源：http://ruq.jlsjyb.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hde.xuanzx.com

Ruby: def to_s; @name; end
来源：http://nzv.zhengqikj.top

C#:   public override string ToString() => Name;
来源：http://yub.tian-w.cn

[G13] 判断对象类型
来源：http://dqc.andypj.xyz

Py:   isinstance(u, User)
来源：http://mjk.cashguo.top

PHP:  $u instanceof User
来源：http://xwr.tanke756.top

JS:   u instanceof User
来源：http://hps.xuetiantiany.cn

TS:   u instanceof User
来源：http://pix.hnqzz.top

Java: u instanceof User
来源：http://cey.gotoacloud.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://cmk.sysykeji.top

Ruby: u.is_a?(User)
来源：http://myn.havefunace.top

C#:   u is User
来源：http://wrx.gaohongyu789.top

[G14] 数据类 / record
来源：http://zxh.havefunace.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sge.hysaishi.cn

PHP:  // 用 readonly 属性模拟
来源：http://rhu.yangfankeji.com

JS:   // 无内置：普通类或对象字面量
来源：http://cuv.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://hhg.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://ady.cheryme.top

Go:   type User struct { Name string; Age int }
来源：http://lgw.hnqzz.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vld.cucudq.cn

C#:   record User(string Name, int Age);
来源：http://qlx.zhengqikj.top

[G15] 枚举
来源：http://mbc.cashguo.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yad.svipenyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bwy.ehwqpu.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lbq.haohaochexian.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://orl.snrcjt.cn

Java: enum Color { RED, GREEN }
来源：http://vaz.hongshengwenyu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://spm.pengpengdd.cyou

Ruby: Color = %i[red green].freeze
来源：http://ysz.tarul.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uad.meibo888.top

[G16] 对象转数组 / 字典
来源：http://wvn.xingfuxueyuan.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uia.zhijiandao.cn

PHP:  get_object_vars($obj);
来源：http://thh.shangyingyoupin.top

JS:   Object.entries(obj)
来源：http://dfh.ivvv.top

TS:   Object.entries(obj)
来源：http://gag.jinyuanbaomall.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bov.zhiwuduotai.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vvv.hongshengwenyu.top

Ruby: obj.instance_variables
来源：http://fns.chenzaomai.com

C#:   // 用反射或 System.Text.Json
来源：http://vhh.yvedp.cn

================================================================================
来源：http://xmd.yonumen.top

H. 异常与错误处理
来源：http://siz.yj202588.top

================================================================================
来源：http://utj.hcnkem.com

[H01] try / catch 基础
来源：http://rjt.epnwcf.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dlz.jqgufenzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://swv.pycfn.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zft.jinqigfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wui.fktsv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kpy.smart0.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mwh.havefunace.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mvb.xingfuxueyuan.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://big.zhiwuduotai.top

[H02] finally / ensure 收尾
来源：http://spj.hnxiangtu.top

Py:   try: f()⏎finally: cleanup()
来源：http://ufp.guowangkeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://lxh.ywan-chungtsiang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jdr.shanyushiyangtech.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qwc.guowangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://obq.hesvh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://upl.vehdjk.com

Ruby: begin; f; ensure; cleanup; end
来源：http://yrd.9152youxi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bly.gogol.net.cn

[H03] 主动抛出异常
来源：http://tdp.xuetiantiany.cn

Py:   raise ValueError("错误信息")
来源：http://mmp.quarkkingdee.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qdf.zhiwuduotai.top

JS:   throw new Error("错误信息");
来源：http://ypn.xziqi.cn

TS:   throw new Error("错误信息");
来源：http://mon.guannengcc.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lto.cheryme.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://igb.zdqjudy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ovp.yonumen.top

C#:   throw new ArgumentException("错误信息");
来源：http://pba.daria6918.cn

[H04] 自定义异常类型
来源：http://zzu.yj20258.top

Py:   class MyError(Exception): pass
来源：http://zud.xuetiantiany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bdf.sysykeji.top

JS:   class MyError extends Error {}
来源：http://hwn.9152youxi.cn

TS:   class MyError extends Error {}
来源：http://uvi.ctjpmb.com

Java: class MyException extends RuntimeException {}
来源：http://pnw.gzhubu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ktm.gaohongyu789.top

Ruby: class MyError < StandardError; end
来源：http://xgl.epnwcf.com

C#:   class MyException : Exception {}
来源：http://gnw.xziqi.cn

[H05] 捕获特定类型
来源：http://vyk.xylfe.cn

Py:   except ValueError as e:
来源：http://flq.ywan-chungtsiang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ajm.0kj1m.cn

JS:   if (e instanceof TypeError) {}
来源：http://iqb.jinyuanbaomall.cn

TS:   if (e instanceof TypeError) {}
来源：http://zzv.gogol.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://bjx.yvedp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mwf.9152youxi.cn

Ruby: rescue ArgumentError => e
来源：http://dfz.xuetiantiany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://job.jyoumei.cn

[H06] 可选值 / 空值安全访问
来源：http://kyg.fzhhl.top

Py:   value = d.get("k") or default
来源：http://muo.yuxming.cn

PHP:  $v = $d["k"] ?? null;
来源：http://keo.guannengcc.top

JS:   obj?.a?.b;  d ?? default
来源：http://uxu.dashuyun.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sjt.ybcxt.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oyz.nanxuanxn.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ciq.316326.xyz

Ruby: d&.dig(:a, :b)
来源：http://zpf.bbcook.cn

C#:   obj?.A?.B ?? default
来源：http://ock.ppjwa.cn

[H07] 断言
来源：http://qgo.jinyuanbaomall.cn

Py:   assert x > 0, "必须为正"
来源：http://jjp.xziqi.cn

PHP:  assert($x > 0);
来源：http://pqm.quarkkingdee.top

JS:   console.assert(x > 0);
来源：http://yvw.redwolf501.top

TS:   console.assert(x > 0);
来源：http://rqd.sysykeji.top

Java: assert x > 0 : "必须为正";
来源：http://lli.feifeiyinyue.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sxx.zhengqikj.top

Ruby: raise "必须为正" unless x > 0
来源：http://yzz.shanyushiyangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://tol.zhijiandao.cn

[H08] 获取错误信息与堆栈
来源：http://ckn.zhengqikj.top

Py:   str(e);  traceback.format_exc()
来源：http://fqe.snrcjt.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gxb.kuanghao11.cn

JS:   e.message;  e.stack
来源：http://ind.xingfuxueyuan.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://kgs.mhx1999.top

Java: e.getMessage();  e.printStackTrace()
来源：http://lem.fzhhl.top

Go:   err.Error()
来源：http://zjd.zhoulong.xyz

Ruby: e.message;  e.backtrace
来源：http://mof.kuanghao11.cn

C#:   e.Message;  e.StackTrace
来源：http://ijq.jinqigufen.top

[H09] 带错误码的异常
来源：http://hsv.fktsv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wew.gaohongyu789.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lpr.hywenlv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://goe.wangshuangyany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mgq.cucudq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vnf.smart0.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nuu.hnxiangtu.top

Ruby: raise MyError.new("fail", 500)
来源：http://hvv.52xcode.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pcu.aibaodan.cn

[H10] 资源自动释放
来源：http://njj.mhx1999.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vyr.shuidangran.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gag.smart0.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sxo.chenjidiqi.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nbe.xinyue.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uyk.wangshuangyany.cn

Go:   defer f.Close()
来源：http://lso.xingfuxueyuan.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ptj.xuetiantiany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bes.hcnkem.com

================================================================================
来源：http://lpd.cashguo.top

I. 正则表达式
来源：http://zpe.dashuyun.cn

================================================================================
来源：http://hxz.quarkkingdee.top

[I01] 判断是否匹配
来源：http://bpc.jinyuanbaomall.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wsk.ywan-chungtsiang.top

PHP:  preg_match('/\d+/', $s);
来源：http://hkm.bbcook.cn

JS:   /\d+/.test(s)
来源：http://ezo.ppjwa.cn

TS:   /\d+/.test(s)
来源：http://lzk.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lzl.sysykeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zfc.svipenyu.cn

Ruby: s.match?(/\d+/)
来源：http://eaa.jianghu66.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jek.hcnkem.com

[I02] 提取所有匹配
来源：http://mqg.daria6918.cn

Py:   re.findall(r"\d+", s)
来源：http://qui.xuetiantiany.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://diq.cqqwz.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wek.cheryme.top

TS:   s.match(/\d+/g)
来源：http://jhn.fzhhl.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cyu.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bwp.cucudq.cn

Ruby: s.scan(/\d+/)
来源：http://sof.fanxiaobao.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nhu.gotoacloud.top

[I03] 提取捕获分组
来源：http://lsi.shzxlz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iaz.hcnkem.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://haz.smart0.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://umu.ywan-chungtsiang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ubp.gotoacloud.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lfh.daria6918.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pke.xuanzx.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uad.ydzc1.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fka.316326.xyz

[I04] 正则替换
来源：http://sqy.uphjek.com

Py:   re.sub(r"\d+", "#", s)
来源：http://vfw.hongshengwenyu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://prs.xingfuxueyuan.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://mfl.xingfuxueyuan.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://jit.hnqzz.top

Java: s.replaceAll("\\d+", "#")
来源：http://ixt.dashuyun.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vlf.cashguo.top

Ruby: s.gsub(/\d+/, "#")
来源：http://eqy.bbcook.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tfy.yj20258.top

[I05] 按正则拆分
来源：http://piy.sysykeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://pew.yuxming.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lwv.zhixingplan.top

JS:   s.split(/\s*,\s*/)
来源：http://gpo.hfpthk.cn

TS:   s.split(/\s*,\s*/)
来源：http://rst.zhixingplan.top

Java: s.split("\\s*,\\s*")
来源：http://rph.cashguo.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cqh.zhixingplan.top

Ruby: s.split(/\s*,\s*/)
来源：http://jku.wangshuangyany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://elz.dianchejie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sjo.wangdashe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kej.yueranfly.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fml.guowangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sqw.zhiwuduotai.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rjv.sysykeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xii.daria6918.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bmp.sufxvd.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jse.daxiang520.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uow.meibo888.top

[I07] 忽略大小写与多行模式
来源：http://vzd.zhoulong.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yho.sysykeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gwd.gaohongyu789.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ctj.guowangkeji.top

TS:   /error/gim
来源：http://ltz.gaohongyu789.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vnx.zdqjudy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oau.jinghuilouyu.cn

Ruby: s.scan(/error/i)
来源：http://uyw.ybcxt.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iwh.jqgufenzy.top

[I08] 贪婪与非贪婪匹配
来源：http://kot.zhaomingkeji.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://aej.nanxinkj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cjx.fktsv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://slj.tian-w.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://liu.snrcjt.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cqj.cqqwz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xyi.ydzc1.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fnr.zhoulong.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bwr.jinghuilouyu.cn

================================================================================
来源：http://eka.tian-w.cn

J. 日期与时间
来源：http://bnq.ctjpmb.com

================================================================================
来源：http://zqp.sxryk.cn

[J01] 获取当前时间
来源：http://qub.gotoacloud.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://lua.shangyingyoupin.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pog.iojbl.cn

JS:   new Date();  Date.now()
来源：http://sgk.dashuyun.cn

TS:   new Date();  Date.now()
来源：http://fsl.jyoumei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ntz.gzhubu.top

Go:   time.Now()
来源：http://wdt.hnxiangtu.top

Ruby: Time.now
来源：http://zvl.nanxuanxn.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ucm.chenjidiqi.icu

[J02] 格式化输出
来源：http://qod.xylfe.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vqe.yfazqb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hwe.fktsv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://thp.xuetiantiany.cn

TS:   d.toISOString()
来源：http://ddx.yueranfly.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aan.hongshengwenyu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pia.ybcxt.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rik.tianlin.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pva.gotoacloud.top

[J03] 字符串解析为日期
来源：http://poh.52xcode.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tra.yongpay.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hjj.dianchejie.cn

JS:   new Date("2024-01-02")
来源：http://sst.chenlongwang.top

TS:   new Date("2024-01-02")
来源：http://yrh.jqgfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://ghb.gaohongyu789.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qwj.vqdsnc.cn

Ruby: Date.parse("2024-01-02")
来源：http://yyl.smart0.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cxd.c1oappe.top

[J04] 时间戳与日期互转
来源：http://fua.sysykeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xcc.gaohongyu789.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://owv.mhx1999.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tsv.fktsv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lzz.shanyushiyangtech.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://odr.aizwys.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cix.gogol.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dog.birdmap.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://chr.hfpthk.cn

[J05] 时间加减（加 7 天）
来源：http://aig.zycfv.cn

Py:   now + timedelta(days=7)
来源：http://wau.cheryme.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://oqh.bbcook.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vzn.fktsv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uul.cheryme.top

Java: LocalDate.now().plusDays(7)
来源：http://lfq.ctjpmb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xdg.yangfankeji.com

Ruby: Time.now + 7 * 86400
来源：http://pmy.sysykeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://npu.jinghuilouyu.cn

[J06] 计算两时间之差
来源：http://tad.pycfn.com

Py:   (end - start).total_seconds()
来源：http://blg.jinyuanbaomall.cn

PHP:  $end->diff($start)->days;
来源：http://xtl.epnwcf.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ycq.mhx1999.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://izu.zhaomingkeji.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://wlq.uphjek.com

Go:   end.Sub(start).Hours()
来源：http://flb.xuetiantiany.cn

Ruby: end - start                 # 返回秒数
来源：http://rep.shangyingyoupin.top

C#:   (end - start).TotalSeconds
来源：http://jit.hammf.cn

[J07] 比较两个日期
来源：http://oni.dianchejie.cn

Py:   d1 < d2;  d1 == d2
来源：http://xta.hammf.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nmi.chenlongwang.top

JS:   d1.getTime() < d2.getTime()
来源：http://jnb.fzhhl.top

TS:   d1.getTime() < d2.getTime()
来源：http://lwc.kuanghao11.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mum.fehbvm.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fgi.tanke756.top

Ruby: d1 < d2;  d1 == d2
来源：http://zxi.sysykeji.top

C#:   d1 < d2;  d1 == d2
来源：http://hfs.yangfankeji.com

[J08] 提取年月日与星期
来源：http://kda.sweek.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nib.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qgh.jinghuilouyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ylp.yangfankeji.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ojz.gotoacloud.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tbl.hnxiangtu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ulv.shzxlz.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uck.haohaochexian.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bdt.0kj1m.cn

[J09] 时区处理
来源：http://mvg.cucudq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bpi.xylfe.cn


<!-- 参考信息 -->