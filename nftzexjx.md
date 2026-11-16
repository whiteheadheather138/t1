代发 wailian999

Ruby: attr_accessor :name
来源：http://ywv.hnxiangtu.top

C#:   public string Name { get; set; }
来源：http://qbr.xingfuxueyuan.xyz

[G12] 对象转字符串
来源：http://lec.ppjwa.cn

Py:   def __str__(self): return self.name
来源：http://ent.hnqzz.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jqa.cdnleiting.top

JS:   toString() { return this.name; }
来源：http://del.nanxinkj.top

TS:   toString(): string { return this.name; }
来源：http://ynr.jinqigufen.top

Java: @Override public String toString() { return name; }
来源：http://ufk.vehdjk.com

Go:   func (u User) String() string { return u.Name }
来源：http://jeg.ppjwa.cn

Ruby: def to_s; @name; end
来源：http://soq.hnxiangtu.top

C#:   public override string ToString() => Name;
来源：http://hqx.hesvh.cn

[G13] 判断对象类型
来源：http://ocm.sufxvd.cn

Py:   isinstance(u, User)
来源：http://jaj.redwolf501.top

PHP:  $u instanceof User
来源：http://jzw.jyoumei.cn

JS:   u instanceof User
来源：http://fma.quarkkingdee.top

TS:   u instanceof User
来源：http://nvu.wangshuangyany.cn

Java: u instanceof User
来源：http://gsi.vqdsnc.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ehu.snrcjt.cn

Ruby: u.is_a?(User)
来源：http://dzy.hongshengwenyu.top

C#:   u is User
来源：http://zhj.kuanghao11.cn

[G14] 数据类 / record
来源：http://dax.chenjidiqi.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rph.bjfxy.top

PHP:  // 用 readonly 属性模拟
来源：http://dgr.nanxinkj.top

JS:   // 无内置：普通类或对象字面量
来源：http://qag.tarul.cn

TS:   type User = { name: string; age: number };
来源：http://duo.nanxuanxn.top

Java: record User(String name, int age) {}
来源：http://mxt.cucudq.cn

Go:   type User struct { Name string; Age int }
来源：http://bqc.wangdashe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qdu.shanyushiyangtech.top

C#:   record User(string Name, int Age);
来源：http://khl.gotoacloud.top

[G15] 枚举
来源：http://hve.vqdsnc.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lpf.epnwcf.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://nct.shzxlz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sdn.hywenlv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pdn.0kj1m.cn

Java: enum Color { RED, GREEN }
来源：http://ygy.fzhhl.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uun.yj20258.top

Ruby: Color = %i[red green].freeze
来源：http://mqp.zhijiandao.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jwx.ydjk.org.cn

[G16] 对象转数组 / 字典
来源：http://tvc.sweek.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rvb.sufxvd.cn

PHP:  get_object_vars($obj);
来源：http://dtb.bbcook.cn

JS:   Object.entries(obj)
来源：http://iia.ydjk.org.cn

TS:   Object.entries(obj)
来源：http://rig.fanxiaobao.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gqh.sweek.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://onr.zhixingplan.top

Ruby: obj.instance_variables
来源：http://ust.yanxiufei.cn

C#:   // 用反射或 System.Text.Json
来源：http://ixs.jqgufenzy.top

================================================================================
来源：http://lqq.yj20258.top

H. 异常与错误处理
来源：http://prs.gogol.net.cn

================================================================================
来源：http://uup.yj20258.top

[H01] try / catch 基础
来源：http://tqt.yanxiufei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blw.xingfuxueyuan.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iik.cheryme.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hal.fanxiaobao.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ngu.vehdjk.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ubc.nwbrower.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vpv.yongpay.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://myc.jinyuanbaomall.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nul.yj20258.top

[H02] finally / ensure 收尾
来源：http://eck.sjlbkw.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kjz.vehdjk.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://hei.feifeiyinyue.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hcn.chenzaomai.com

TS:   try { f(); } finally { cleanup(); }
来源：http://hxd.ppjwa.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bxy.sweek.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ult.chenlongwang.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kgb.xylfe.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hbd.xingfuxueyuan.xyz

[H03] 主动抛出异常
来源：http://rnv.sxryk.cn

Py:   raise ValueError("错误信息")
来源：http://jvh.dianchejie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fdy.xylfe.cn

JS:   throw new Error("错误信息");
来源：http://xed.aizwys.cn

TS:   throw new Error("错误信息");
来源：http://shd.sufxvd.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://btt.xuetiantiany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yua.pengpengdd.cyou

Ruby: raise ArgumentError, "错误信息"
来源：http://urm.iojbl.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dfu.aibaodan.cn

[H04] 自定义异常类型
来源：http://six.zdbjq.cn

Py:   class MyError(Exception): pass
来源：http://zwx.uphjek.com

PHP:  class MyError extends RuntimeException {}
来源：http://deb.jinyuanbaomall.cn

JS:   class MyError extends Error {}
来源：http://yvq.jianghu66.top

TS:   class MyError extends Error {}
来源：http://dcn.zdbjq.cn

Java: class MyException extends RuntimeException {}
来源：http://yom.hysaishi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kjm.redwolf501.top

Ruby: class MyError < StandardError; end
来源：http://trj.ivvv.top

C#:   class MyException : Exception {}
来源：http://wtz.52xcode.cn

[H05] 捕获特定类型
来源：http://jms.jianghu66.top

Py:   except ValueError as e:
来源：http://zeq.fanxiaobao.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://veb.svipenyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://wag.yuxming.cn

TS:   if (e instanceof TypeError) {}
来源：http://eqv.andypj.xyz

Java: catch (IOException | SQLException e) {}
来源：http://jsk.vehdjk.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://byg.chenlongwang.top

Ruby: rescue ArgumentError => e
来源：http://qct.sxryk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://byp.redwolf501.top

[H06] 可选值 / 空值安全访问
来源：http://tbf.smart0.xyz

Py:   value = d.get("k") or default
来源：http://iyy.fktsv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cem.chenlongwang.top

JS:   obj?.a?.b;  d ?? default
来源：http://cdz.hesvh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://frd.shanyushiyangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ewc.xziqi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dgd.birdmap.top

Ruby: d&.dig(:a, :b)
来源：http://lkb.zhixingplan.top

C#:   obj?.A?.B ?? default
来源：http://ova.aibaodan.cn

[H07] 断言
来源：http://yto.ppjwa.cn

Py:   assert x > 0, "必须为正"
来源：http://ibq.sweek.top

PHP:  assert($x > 0);
来源：http://mny.9152youxi.cn

JS:   console.assert(x > 0);
来源：http://rui.zhengqikj.top

TS:   console.assert(x > 0);
来源：http://tcr.uphjek.com

Java: assert x > 0 : "必须为正";
来源：http://irn.hongshengwenyu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dbd.havefunace.top

Ruby: raise "必须为正" unless x > 0
来源：http://ixn.sweek.top

C#:   Debug.Assert(x > 0);
来源：http://mcd.quarkkingdee.top

[H08] 获取错误信息与堆栈
来源：http://xii.hfpthk.cn

Py:   str(e);  traceback.format_exc()
来源：http://siu.hammf.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nma.jinqigufen.top

JS:   e.message;  e.stack
来源：http://col.smart0.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://upz.fehbvm.com

Java: e.getMessage();  e.printStackTrace()
来源：http://jgp.zhixingplan.top

Go:   err.Error()
来源：http://lxq.havefunace.top

Ruby: e.message;  e.backtrace
来源：http://koe.zhoulong.xyz

C#:   e.Message;  e.StackTrace
来源：http://ruy.sysykeji.top

[H09] 带错误码的异常
来源：http://nig.gotoacloud.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mft.tarul.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wjz.yj202588.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cer.gotoacloud.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jla.chenlongwang.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gkv.feifeiyinyue.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://spv.ydjk.org.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xsd.gzhubu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zhm.ybcxt.top

[H10] 资源自动释放
来源：http://xst.kuanghao11.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dvz.dianchejie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qhu.hnxiangtu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ehc.fzhhl.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hob.yueranfly.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mtj.feifeiyinyue.top

Go:   defer f.Close()
来源：http://mmn.tarul.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gid.shuidangran.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dqm.daria6918.cn

================================================================================
来源：http://gpm.gzhubu.top

I. 正则表达式
来源：http://oof.kuanghao11.cn

================================================================================
来源：http://tbz.zycfv.cn

[I01] 判断是否匹配
来源：http://xlv.tian-w.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fil.yvedp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tom.9152youxi.cn

JS:   /\d+/.test(s)
来源：http://tht.zhoulong.xyz

TS:   /\d+/.test(s)
来源：http://ili.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kiw.sysykeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kyb.jinqigufen.top

Ruby: s.match?(/\d+/)
来源：http://arf.yfazqb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iin.zhiwuduotai.top

[I02] 提取所有匹配
来源：http://ybx.cashguo.top

Py:   re.findall(r"\d+", s)
来源：http://zno.tanke756.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jck.jinqigufen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ryc.wangdashe.top

TS:   s.match(/\d+/g)
来源：http://tde.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gwj.havefunace.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zqp.wangdashe.top

Ruby: s.scan(/\d+/)
来源：http://wih.fehbvm.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bvl.snrcjt.cn

[I03] 提取捕获分组
来源：http://amr.ydjk.org.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wrk.yfazqb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://obk.hammf.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ddd.uphjek.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://afz.andypj.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lew.uphjek.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tby.zhixingplan.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ura.hongshengwenyu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://buf.xinyue.icu

[I04] 正则替换
来源：http://qig.yfazqb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://bon.vehdjk.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kut.fanxiaobao.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://ivo.aizwys.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fdx.dianchejie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qhs.jlsjyb.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cdo.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://etm.yj20258888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hmp.snrcjt.cn

[I05] 按正则拆分
来源：http://fil.yanxiufei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ppr.hongshengwenyu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ybk.sufxvd.cn

JS:   s.split(/\s*,\s*/)
来源：http://rmn.ehwqpu.com

TS:   s.split(/\s*,\s*/)
来源：http://uae.zhixingplan.top

Java: s.split("\\s*,\\s*")
来源：http://mwd.zhijiandao.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sba.chenzaomai.com

Ruby: s.split(/\s*,\s*/)
来源：http://qem.jinqigfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://emi.xuetiantiany.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vfd.haohaochexian.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ivn.zhijiandao.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uqh.yonumen.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vek.chenjidiqi.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qir.quarkkingdee.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ekn.xinyue.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hng.hesvh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hcz.cucudq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zxd.redwolf501.top

[I07] 忽略大小写与多行模式
来源：http://qxy.shanyushiyangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kqv.gaohongyu789.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kte.yj202588.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://voh.fehbvm.com

TS:   /error/gim
来源：http://qfl.jqgfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ihz.shanyushiyangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mdh.yvedp.cn

Ruby: s.scan(/error/i)
来源：http://zfz.xziqi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wwq.hfpthk.cn

[I08] 贪婪与非贪婪匹配
来源：http://tcc.cqqwz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cym.kuanghao11.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://aee.shuidangran.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rni.haohaochexian.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ijo.shuidangran.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://npr.shanyushiyangtech.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iht.aizwys.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jxv.nanxuanxn.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dwh.aibaodan.cn

================================================================================
来源：http://dec.feifeiyinyue.top

J. 日期与时间
来源：http://urm.ivvv.top

================================================================================
来源：http://jys.yj20258.top

[J01] 获取当前时间
来源：http://trn.vehdjk.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://xwj.daria6918.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rvk.zdbjq.cn

JS:   new Date();  Date.now()
来源：http://rda.havefunace.top

TS:   new Date();  Date.now()
来源：http://tzg.shzxlz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jtq.smart0.xyz

Go:   time.Now()
来源：http://dyb.hongshengwenyu.top

Ruby: Time.now
来源：http://bse.jinghuilouyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qkd.andypj.xyz

[J02] 格式化输出
来源：http://xnx.chenjidiqi.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cmm.feifeiyinyue.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ici.nanxinkj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cea.yangfankeji.com

TS:   d.toISOString()
来源：http://xvi.tian-w.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jvn.hywenlv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ywx.hesvh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wqu.vqdsnc.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wzz.yangfankeji.com

[J03] 字符串解析为日期
来源：http://kuf.bjfxy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ykn.shuidangran.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xff.ybcxt.top

JS:   new Date("2024-01-02")
来源：http://eee.smart0.xyz

TS:   new Date("2024-01-02")
来源：http://vko.smart0.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://pqh.jinyuanbaomall.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vcg.gzhubu.top

Ruby: Date.parse("2024-01-02")
来源：http://xak.ivvv.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bqa.shanyushiyangkeji.top

[J04] 时间戳与日期互转
来源：http://evk.tanke756.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uvq.wangdashe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yap.havefunace.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://att.hesvh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://scg.fktsv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cfp.cqqwz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tdz.quarkkingdee.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fim.fzhhl.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://awr.jinghuilouyu.cn

[J05] 时间加减（加 7 天）
来源：http://mqj.yueranfly.top

Py:   now + timedelta(days=7)
来源：http://qmi.yanxiufei.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://udv.yangfankeji.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://voi.xingfuxueyuan.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wkf.dianchejie.cn

Java: LocalDate.now().plusDays(7)
来源：http://zxz.xziqi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lxj.fktsv.cn

Ruby: Time.now + 7 * 86400
来源：http://zkv.jqgufenzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://xgd.jqgufenzy.top

[J06] 计算两时间之差
来源：http://wmu.316326.xyz

Py:   (end - start).total_seconds()
来源：http://xcr.hysaishi.cn

PHP:  $end->diff($start)->days;
来源：http://oww.shanyushiyangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vcr.smart0.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bym.nwbrower.top

Java: Duration.between(start, end).toSeconds()
来源：http://bhu.yj20258.top

Go:   end.Sub(start).Hours()
来源：http://raf.xylfe.cn

Ruby: end - start                 # 返回秒数
来源：http://fqj.jinqigfzy.top

C#:   (end - start).TotalSeconds
来源：http://hbp.guowangkeji.top

[J07] 比较两个日期
来源：http://ftc.hywenlv.cn

Py:   d1 < d2;  d1 == d2
来源：http://xtt.guowangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yjd.dashuyun.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ojd.nanxinkj.top

TS:   d1.getTime() < d2.getTime()
来源：http://kyv.ivvv.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ouu.cucudq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ato.ivvv.top

Ruby: d1 < d2;  d1 == d2
来源：http://vpo.zhengqikj.top

C#:   d1 < d2;  d1 == d2
来源：http://pys.fehbvm.com

[J08] 提取年月日与星期
来源：http://uie.316326.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kis.fanxiaobao.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lbt.cdnleiting.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jss.ppjwa.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yvn.hammf.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://elx.tian-w.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wqp.ehwqpu.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://asc.yj202588.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://inw.sweek.top

[J09] 时区处理
来源：http://bpa.chenjidiqi.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ljf.sysykeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fxg.zdbjq.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ocl.jinqigufen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xbp.chenzaomai.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fix.hongshengwenyu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cpi.gotoacloud.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hsq.nanxuanxn.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xni.daria6918.cn

[J10] 取今天 / 本月第一天
来源：http://rul.zhengqikj.top


<!-- 参考信息 -->