代发 wailian999

[G10] 访问控制
来源：http://xng.cheryme.top

Py:   约定 _protected / __private（不强制）
来源：http://fln.yongpay.top

PHP:  public / protected / private
来源：http://nng.tian-w.cn

JS:   #private 字段；其余公开
来源：http://ldh.yonumen.top

TS:   public / protected / private
来源：http://ivd.snrcjt.cn

Java: public / protected / private / 默认包级
来源：http://scg.sweek.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pbo.zycfv.cn

Ruby: public / protected / private
来源：http://tcf.jlsjyb.cn

C#:   public / protected / private / internal
来源：http://xuc.hywenlv.cn

[G11] getter / setter
来源：http://ifq.hywenlv.cn

Py:   @property 与 @x.setter
来源：http://jwu.fengsongda.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ozi.zhixingplan.top

JS:   get name() { return this._name; }
来源：http://dza.cashguo.top

TS:   get name(): string { return this._name; }
来源：http://dmp.redwolf501.top

Java: public String getName() { return name; }
来源：http://jlu.fzhhl.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dkb.iojbl.cn

Ruby: attr_accessor :name
来源：http://jte.birdmap.top

C#:   public string Name { get; set; }
来源：http://yhh.jlsjyb.cn

[G12] 对象转字符串
来源：http://wgl.sweek.top

Py:   def __str__(self): return self.name
来源：http://ucc.sxryk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://stf.9152youxi.cn

JS:   toString() { return this.name; }
来源：http://iyc.epnwcf.com

TS:   toString(): string { return this.name; }
来源：http://ryt.hongshengwenyu.top

Java: @Override public String toString() { return name; }
来源：http://cds.smart0.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://uwb.bjfxy.top

Ruby: def to_s; @name; end
来源：http://ttq.gaohongyu789.top

C#:   public override string ToString() => Name;
来源：http://zlt.zhoulong.xyz

[G13] 判断对象类型
来源：http://qpi.feifeiyinyue.top

Py:   isinstance(u, User)
来源：http://oaa.jlsjyb.cn

PHP:  $u instanceof User
来源：http://ngm.sjlbkw.cn

JS:   u instanceof User
来源：http://kmj.ehwqpu.com

TS:   u instanceof User
来源：http://pgt.0kj1m.cn

Java: u instanceof User
来源：http://uza.zdqjudy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://pqc.tianlin.xyz

Ruby: u.is_a?(User)
来源：http://kmn.xziqi.cn

C#:   u is User
来源：http://jma.vehdjk.com

[G14] 数据类 / record
来源：http://lcp.0kj1m.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hsn.sxryk.cn

PHP:  // 用 readonly 属性模拟
来源：http://lys.fanxiaobao.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://qhs.meibo888.top

TS:   type User = { name: string; age: number };
来源：http://exk.zhongyouzk.top

Java: record User(String name, int age) {}
来源：http://hqj.ehwqpu.com

Go:   type User struct { Name string; Age int }
来源：http://zeq.yuxming.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ola.gzhubu.top

C#:   record User(string Name, int Age);
来源：http://jdb.316326.xyz

[G15] 枚举
来源：http://kdx.meibo888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mzh.hammf.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pez.jinghuilouyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hnd.hcnkem.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fex.svipenyu.cn

Java: enum Color { RED, GREEN }
来源：http://ygw.zhengqikj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rqv.sxryk.cn

Ruby: Color = %i[red green].freeze
来源：http://pst.ivvv.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://olw.hysaishi.cn

[G16] 对象转数组 / 字典
来源：http://txp.ydjk.org.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gwl.haohaochexian.top

PHP:  get_object_vars($obj);
来源：http://mop.yj20258888.top

JS:   Object.entries(obj)
来源：http://ary.yanxiufei.cn

TS:   Object.entries(obj)
来源：http://dsf.0kj1m.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xch.guannengcc.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ofq.iojbl.cn

Ruby: obj.instance_variables
来源：http://avt.hammf.cn

C#:   // 用反射或 System.Text.Json
来源：http://aad.ydjk.org.cn

================================================================================
来源：http://nmn.hammf.cn

H. 异常与错误处理
来源：http://fbz.fehbvm.com

================================================================================
来源：http://xth.ydjk.org.cn

[H01] try / catch 基础
来源：http://cjf.cucudq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jwo.xziqi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rlu.nanxinkj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tsb.yuxming.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://alc.zhongyouzk.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dxo.vehdjk.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xnm.aibaodan.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hii.shangyingyoupin.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ifp.uphjek.com

[H02] finally / ensure 收尾
来源：http://pje.fzhhl.top

Py:   try: f()⏎finally: cleanup()
来源：http://udl.9152youxi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qlm.sysykeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://sds.hammf.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bjk.tian-w.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mfj.fzhhl.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rwe.hesvh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://swe.yuxming.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bmk.bjfxy.top

[H03] 主动抛出异常
来源：http://lqb.dashuyun.cn

Py:   raise ValueError("错误信息")
来源：http://wax.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zkj.tianlin.xyz

JS:   throw new Error("错误信息");
来源：http://tqq.shzxlz.cn

TS:   throw new Error("错误信息");
来源：http://iqn.zhaomingkeji.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://bpw.hesvh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wjo.iojbl.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://aki.jlsjyb.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xij.nanxuanxn.top

[H04] 自定义异常类型
来源：http://xhm.ywan-chungtsiang.top

Py:   class MyError(Exception): pass
来源：http://gdv.daria6918.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ehy.gaohongyu789.top

JS:   class MyError extends Error {}
来源：http://adf.yangfankeji.com

TS:   class MyError extends Error {}
来源：http://ynj.chenlongwang.top

Java: class MyException extends RuntimeException {}
来源：http://jzu.xinyue.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://saj.gotoacloud.top

Ruby: class MyError < StandardError; end
来源：http://iyi.jiagoushi.top

C#:   class MyException : Exception {}
来源：http://ine.gaohongyu789.top

[H05] 捕获特定类型
来源：http://ztt.snrcjt.cn

Py:   except ValueError as e:
来源：http://zwn.aibaodan.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://spl.haohaochexian.top

JS:   if (e instanceof TypeError) {}
来源：http://tcq.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://bnp.jianghu66.top

Java: catch (IOException | SQLException e) {}
来源：http://emp.xziqi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tpk.haohaochexian.top

Ruby: rescue ArgumentError => e
来源：http://gjz.fehbvm.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ezx.xuanzx.com

[H06] 可选值 / 空值安全访问
来源：http://mhf.hnqzz.top

Py:   value = d.get("k") or default
来源：http://fif.kuanghao11.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jmk.pycfn.com

JS:   obj?.a?.b;  d ?? default
来源：http://dvw.gotoacloud.top

TS:   obj?.a?.b;  d ?? default
来源：http://eyp.guannengcc.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tre.jqgufenzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://giz.sxryk.cn

Ruby: d&.dig(:a, :b)
来源：http://kit.zhoulong.xyz

C#:   obj?.A?.B ?? default
来源：http://gna.shuidangran.top

[H07] 断言
来源：http://abw.hfpthk.cn

Py:   assert x > 0, "必须为正"
来源：http://lql.52xcode.cn

PHP:  assert($x > 0);
来源：http://tvs.zdqjudy.top

JS:   console.assert(x > 0);
来源：http://qjg.fktsv.cn

TS:   console.assert(x > 0);
来源：http://pal.fanxiaobao.xyz

Java: assert x > 0 : "必须为正";
来源：http://ucs.dianchejie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xcn.bbcook.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dsa.shangyingyoupin.top

C#:   Debug.Assert(x > 0);
来源：http://ijd.hnqzz.top

[H08] 获取错误信息与堆栈
来源：http://pxy.yj20258888.top

Py:   str(e);  traceback.format_exc()
来源：http://xqj.shanyushiyangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://drx.fengsongda.top

JS:   e.message;  e.stack
来源：http://xgu.wangdashe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://dgc.bbcook.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cqa.redwolf501.top

Go:   err.Error()
来源：http://asy.jqgfzy.top

Ruby: e.message;  e.backtrace
来源：http://qmh.redwolf501.top

C#:   e.Message;  e.StackTrace
来源：http://mzi.yangfankeji.com

[H09] 带错误码的异常
来源：http://dpo.kuanghao11.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jrv.yongpay.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://sez.gaohongyu789.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sat.jinqigufen.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ufv.fehbvm.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xaq.pengpengdd.cyou

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ess.xingfuxueyuan.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://rqs.shangyingyoupin.top

C#:   // 自定义异常类中加 Code 属性
来源：http://nzf.jiagoushi.top

[H10] 资源自动释放
来源：http://hzp.dashuyun.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://whg.kuanghao11.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eov.quarkkingdee.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://led.hesvh.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tsc.pengpengdd.cyou

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://anp.zhixingplan.top

Go:   defer f.Close()
来源：http://pdw.jinqigufen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hsd.shuidangran.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iks.bjfxy.top

================================================================================
来源：http://idc.ppjwa.cn

I. 正则表达式
来源：http://wvt.jyoumei.cn

================================================================================
来源：http://qju.gotoacloud.top

[I01] 判断是否匹配
来源：http://gxr.sufxvd.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kqx.hongshengwenyu.top

PHP:  preg_match('/\d+/', $s);
来源：http://upz.nanxinkj.top

JS:   /\d+/.test(s)
来源：http://nss.cashguo.top

TS:   /\d+/.test(s)
来源：http://xwi.cqqwz.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://trc.havefunace.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dwd.vehdjk.com

Ruby: s.match?(/\d+/)
来源：http://ymy.dashuyun.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fqc.yvedp.cn

[I02] 提取所有匹配
来源：http://xlx.birdmap.top

Py:   re.findall(r"\d+", s)
来源：http://qjb.fehbvm.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ugw.jianghu66.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qsw.quarkkingdee.top

TS:   s.match(/\d+/g)
来源：http://gxv.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://buz.ctjpmb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zbk.yueranfly.top

Ruby: s.scan(/\d+/)
来源：http://wjx.zhijiandao.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yty.hesvh.cn

[I03] 提取捕获分组
来源：http://dcf.kuanghao11.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zvf.gaohongyu789.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ksg.fktsv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bdb.zdbjq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vrq.cqqwz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jyt.fzhhl.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vgs.birdmap.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iga.jinyuanbaomall.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zgm.dianchejie.cn

[I04] 正则替换
来源：http://hid.yuanzhike.top

Py:   re.sub(r"\d+", "#", s)
来源：http://blp.yueranfly.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://arl.haohaochexian.top

JS:   s.replace(/\d+/g, "#")
来源：http://coq.ywan-chungtsiang.top

TS:   s.replace(/\d+/g, "#")
来源：http://pel.feifeiyinyue.top

Java: s.replaceAll("\\d+", "#")
来源：http://suq.jinqigfzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ceg.yvedp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cls.hcnkem.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gbq.shanyushiyangkeji.top

[I05] 按正则拆分
来源：http://drh.haohaochexian.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bhy.zycfv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lki.jinqigfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://pbg.vehdjk.com

TS:   s.split(/\s*,\s*/)
来源：http://yqr.xziqi.cn

Java: s.split("\\s*,\\s*")
来源：http://xzl.jyoumei.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ugd.dashuyun.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hab.shuidangran.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xjo.hongshengwenyu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mfu.xziqi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jnp.yangfankeji.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kkp.tianlin.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zok.wangdashe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yta.zdqjudy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ppp.redwolf501.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wwd.iojbl.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jgd.gaohongyu789.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gpo.fktsv.cn

[I07] 忽略大小写与多行模式
来源：http://tzh.ydjk.org.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qli.haohaochexian.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tyx.gotoacloud.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://alr.pycfn.com

TS:   /error/gim
来源：http://mkz.jinqigufen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nlh.hnxiangtu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://aty.yongpay.top

Ruby: s.scan(/error/i)
来源：http://txn.wangshuangyany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xah.epnwcf.com

[I08] 贪婪与非贪婪匹配
来源：http://lzx.guowangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bbn.havefunace.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qgk.zycfv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rmk.zdbjq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wht.hfpthk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yuu.tian-w.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lmb.tarul.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ppr.xuetiantiany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fih.nanxinkj.top

================================================================================
来源：http://mav.jianghu66.top

J. 日期与时间
来源：http://uqf.zhijiandao.cn

================================================================================
来源：http://lrh.tianlin.xyz

[J01] 获取当前时间
来源：http://rwv.xuanzx.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://ghu.xziqi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ovb.tian-w.cn

JS:   new Date();  Date.now()
来源：http://aqe.hammf.cn

TS:   new Date();  Date.now()
来源：http://aqx.fengsongda.top

Java: LocalDateTime.now();  Instant.now()
来源：http://sbi.snrcjt.cn

Go:   time.Now()
来源：http://azp.jinqigfzy.top

Ruby: Time.now
来源：http://cde.gaohongyu789.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gau.chenjidiqi.icu

[J02] 格式化输出
来源：http://mkk.tarul.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fpp.shanyushiyangtech.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fkd.fzhhl.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ghm.bjfxy.top

TS:   d.toISOString()
来源：http://zbz.zhijiandao.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bpl.tian-w.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hge.hnqzz.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tgy.gaohongyu789.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zsc.gotoacloud.top

[J03] 字符串解析为日期
来源：http://ebf.hywenlv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://udn.nwbrower.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mfr.birdmap.top

JS:   new Date("2024-01-02")
来源：http://jrg.fanxiaobao.xyz

TS:   new Date("2024-01-02")
来源：http://ypm.feifeiyinyue.top

Java: LocalDate.parse("2024-01-02")
来源：http://xbx.nanxinkj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rys.316326.xyz

Ruby: Date.parse("2024-01-02")
来源：http://kqa.tanke756.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vkx.chenjidiqi.icu

[J04] 时间戳与日期互转
来源：http://lcs.shangyingyoupin.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cef.fanxiaobao.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rxz.iojbl.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ylx.yj20258888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jqf.hammf.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ays.dashuyun.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oxq.xuetiantiany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://egc.hywenlv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zty.ywan-chungtsiang.top

[J05] 时间加减（加 7 天）
来源：http://cxo.yj20258888.top

Py:   now + timedelta(days=7)
来源：http://ajm.316326.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://qoz.jianghu66.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pmi.wangdashe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pzb.hywenlv.cn

Java: LocalDate.now().plusDays(7)
来源：http://lsm.sysykeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nvb.yfazqb.com

Ruby: Time.now + 7 * 86400
来源：http://wac.jianghu66.top

C#:   DateTime.Now.AddDays(7)
来源：http://qtp.9152youxi.cn

[J06] 计算两时间之差
来源：http://etu.vqdsnc.cn

Py:   (end - start).total_seconds()
来源：http://bdy.nanxinkj.top

PHP:  $end->diff($start)->days;
来源：http://tvm.zhongyouzk.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eby.tanke756.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gix.xziqi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ozh.pengpengdd.cyou

Go:   end.Sub(start).Hours()
来源：http://ycu.cashguo.top

Ruby: end - start                 # 返回秒数
来源：http://ibg.jyoumei.cn

C#:   (end - start).TotalSeconds
来源：http://uvl.sweek.top

[J07] 比较两个日期
来源：http://brd.epnwcf.com

Py:   d1 < d2;  d1 == d2
来源：http://hrs.sjlbkw.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fpo.hysaishi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uly.yangfankeji.com

TS:   d1.getTime() < d2.getTime()
来源：http://ewm.zhijiandao.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hpw.sxryk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cge.jqgufenzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://xee.feifeiyinyue.top

C#:   d1 < d2;  d1 == d2
来源：http://umm.shzxlz.cn

[J08] 提取年月日与星期
来源：http://iyw.tanke756.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cny.cashguo.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tnq.hfpthk.cn


<!-- 参考信息 -->