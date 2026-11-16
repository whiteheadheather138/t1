代发 wailian999

[Q78] 当前时间
来源：http://tsq.gogol.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gbx.jqgufenzy.top

[Q79] 字符串拼接
来源：http://tyr.ydjk.org.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fca.hcnkem.com

[Q80] 字符串截取
来源：http://jan.cheryme.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://irp.shuidangran.top

[Q81] 字符串替换
来源：http://ihw.cdnleiting.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://owp.sysykeji.top

[Q82] 字符长度与字节长度
来源：http://yoj.cheryme.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zve.quarkkingdee.top

[Q83] 大小写转换
来源：http://art.sysykeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xsg.yuanzhike.top

[Q84] 去除首尾空格
来源：http://lrd.hfpthk.cn

SELECT TRIM(name) FROM users;
来源：http://ajs.andypj.xyz

[Q85] 数值取整
来源：http://qkv.chenjidiqi.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nnu.fzhhl.top

[Q86] 读取 JSON 字段
来源：http://zip.zhoulong.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nms.wangshuangyany.cn

[Q87] JSON 字段做条件
来源：http://wmd.yuxming.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://szn.chenzaomai.com

[Q88] 行转列（条件聚合）
来源：http://hvt.sxryk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xio.ehwqpu.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vhi.yongpay.top

[Q89] 判断表是否存在
来源：http://ukj.fengsongda.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bie.hesvh.cn

[Q90] 生成序号列
来源：http://flf.yj20258888.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://prr.dashuyun.cn

================================================================================
来源：http://mhs.jqgfzy.top

R. Bash 专题
来源：http://iug.sweek.top

================================================================================
来源：http://pvy.jinyuanbaomall.cn

[R01] shebang 与严格模式
来源：http://jek.meibo888.top

#!/usr/bin/env bash
来源：http://gkh.jyoumei.cn

set -euo pipefail
来源：http://uxj.mhx1999.top

[R02] 变量赋值与使用
来源：http://ktb.fanxiaobao.xyz

name="Tom"; echo "$name"
来源：http://tea.jiagoushi.top

[R03] 只读变量
来源：http://yqy.shanyushiyangtech.top

readonly PI=3.14
来源：http://nlz.yuxming.cn

[R04] 位置参数
来源：http://yux.yongpay.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gof.hammf.cn

[R05] 参数默认值
来源：http://rea.shzxlz.cn

name="${1:-default}"
来源：http://ruq.ydjk.org.cn

[R06] 判断命令是否存在
来源：http://ojy.jqgfzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://afm.jqgfzy.top

[R07] if 判断文件
来源：http://bpa.c1oappe.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oce.tanke756.top

[R08] 数值比较
来源：http://hlq.uphjek.com

if (( a > b )); then echo "a 更大"; fi
来源：http://dan.hnqzz.top

[R09] 字符串比较
来源：http://oqf.9152youxi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nph.bbcook.cn

[R10] 正则匹配
来源：http://wfu.zhiwuduotai.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://per.fktsv.cn

[R11] case 多分支
来源：http://lvk.jinyuanbaomall.cn

case "$1" in
来源：http://zos.xuanzx.com

start) echo "启动" ;;
来源：http://bio.xziqi.cn

stop)  echo "停止" ;;
来源：http://ymk.bjfxy.top

*)     echo "未知命令" ;;
来源：http://wqa.jqgfzy.top

esac
来源：http://eef.shzxlz.cn

[R12] for 遍历文件
来源：http://zru.havefunace.top

for f in *.txt; do echo "$f"; done
来源：http://sps.0kj1m.cn

[R13] for 计数循环
来源：http://tdu.cheryme.top

for i in {1..10}; do echo "$i"; done
来源：http://dch.redwolf501.top

[R14] C 风格 for
来源：http://koz.0kj1m.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lor.xingfuxueyuan.xyz

[R15] while 逐行读文件
来源：http://rle.smart0.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nkk.nanxinkj.top

[R16] until 等待条件
来源：http://zra.nwbrower.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ata.yfazqb.com

[R17] 数组定义与取值
来源：http://wca.feifeiyinyue.top

arr=(a b c); echo "${arr[0]}"
来源：http://fkm.shuidangran.top

[R18] 遍历数组
来源：http://bdn.guannengcc.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wsr.jinqigfzy.top

[R19] 数组长度
来源：http://vqg.cashguo.top

echo "${#arr[@]}"
来源：http://bcc.mhx1999.top

[R20] 关联数组（字典）
来源：http://cpf.yonumen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eik.shangyingyoupin.top

[R21] 字符串长度
来源：http://gln.guannengcc.top

echo "${#s}"
来源：http://zvq.hnxiangtu.top

[R22] 截取子串
来源：http://lbe.yfazqb.com

echo "${s:0:5}"
来源：http://bwy.fanxiaobao.xyz

[R23] 字符串替换
来源：http://elj.ctjpmb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fbc.shuidangran.top

[R24] 大小写转换
来源：http://jnn.xuanzx.com

echo "${s^^}"; echo "${s,,}"
来源：http://qto.gaohongyu789.top

[R25] 去后缀 / 去前缀
来源：http://cvd.gotoacloud.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://oqx.guannengcc.top

[R26] 命令替换
来源：http://sxu.hysaishi.cn

now=$(date +%F); echo "$now"
来源：http://leo.nanxinkj.top

[R27] 算术展开
来源：http://eqg.jqgufenzy.top

echo $((1 + 2 * 3))
来源：http://kqc.shanyushiyangkeji.top

[R28] 浮点运算
来源：http://dis.jinqigufen.top

echo "scale=2; 10/3" | bc
来源：http://vbi.aizwys.cn

[R29] 定义函数
来源：http://whs.cdnleiting.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jwn.feifeiyinyue.top

[R30] 函数返回状态码
来源：http://abn.316326.xyz

f() { return 0; }; f || echo "失败了"
来源：http://cbu.fehbvm.com

[R31] 局部变量
来源：http://gsz.316326.xyz

f() { local x=1; echo "$x"; }
来源：http://ccd.feifeiyinyue.top

[R32] 参数个数校验
来源：http://cqa.cucudq.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kpd.tian-w.cn

[R33] 捕获错误并提示行号
来源：http://qtd.mhx1999.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lrd.tian-w.cn

[R34] 退出时清理
来源：http://mms.sjlbkw.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dcv.xziqi.cn

[R35] 后台执行并等待
来源：http://waz.guannengcc.top

sleep 5 & pid=$!; wait "$pid"
来源：http://swf.fzhhl.top

[R36] 并发执行多个任务
来源：http://vrp.daxiang520.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jgd.cashguo.top

[R37] 把输出赋给变量
来源：http://ymv.chenzaomai.com

files=$(ls -1)
来源：http://jxf.jqgufenzy.top

[R38] 管道串联
来源：http://iim.tanke756.top

cat a.txt | grep -i error | wc -l
来源：http://yvi.chenjidiqi.icu

[R39] 重定向标准输出与错误
来源：http://ynj.sxryk.cn

cmd > out.log 2>&1
来源：http://ori.ppjwa.cn

[R40] 追加写日志
来源：http://pyl.chenzaomai.com

echo "log" >> out.log
来源：http://qvg.daxiang520.top

[R41] 丢弃输出
来源：http://svc.ctjpmb.com

cmd >/dev/null 2>&1
来源：http://bst.sjlbkw.cn

[R42] 输入重定向
来源：http://muf.zhengqikj.top

wc -l < a.txt
来源：http://mqh.hesvh.cn

[R43] 按名字查找文件
来源：http://wdb.sjlbkw.cn

find . -name "*.log" -type f
来源：http://gbu.nanxuanxn.top

[R44] 按修改时间查找
来源：http://uks.jianghu66.top

find . -mtime -7 -type f
来源：http://xkj.tanke756.top

[R45] 批量删除
来源：http://and.shanyushiyangkeji.top

find . -name "*.tmp" -delete
来源：http://xxz.fehbvm.com

[R46] 递归替换文件内容
来源：http://ram.fanxiaobao.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wtm.cheryme.top

[R47] sed 单行替换
来源：http://jxm.gotoacloud.top

sed -i 's/foo/bar/g' a.txt
来源：http://mki.zdbjq.cn

[R48] awk 取指定列
来源：http://try.fzhhl.top

awk '{print $1, $3}' a.txt
来源：http://qtu.hywenlv.cn

[R49] awk 带条件
来源：http://fkp.gaohongyu789.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sql.haohaochexian.top

[R50] awk 求和
来源：http://khe.gzhubu.top

awk '{s += $2} END {print s}' a.txt
来源：http://tuu.xuanzx.com

[R51] 排序去重取前几
来源：http://uba.feifeiyinyue.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ema.hywenlv.cn

[R52] 统计行数
来源：http://bov.zhaomingkeji.xyz

wc -l a.txt
来源：http://hdj.c1oappe.top

[R53] 查看文件头与实时尾
来源：http://vfk.yvedp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jcj.chenlongwang.top

[R54] 比较两个文件
来源：http://hdo.wangshuangyany.cn

diff a.txt b.txt
来源：http://cag.dianchejie.cn

[R55] 压缩与解压
来源：http://zak.epnwcf.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dqb.zhoulong.xyz

[R56] 远程拷贝
来源：http://rbj.haohaochexian.top

scp file user@host:/path/
来源：http://ksm.yueranfly.top

[R57] 远程执行命令
来源：http://twz.daria6918.cn

ssh user@host 'uptime'
来源：http://apy.zycfv.cn

[R58] 下载文件
来源：http://tez.fanxiaobao.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dsm.zhijiandao.cn

[R59] 发 POST JSON
来源：http://nal.xinyue.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eia.hnxiangtu.top

[R60] 只看 HTTP 状态码
来源：http://xbm.cashguo.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wlf.dashuyun.cn

[R61] 磁盘占用
来源：http://joz.pengpengdd.cyou

df -h;  du -sh *
来源：http://ioj.zdqjudy.top

[R62] 找最占空间的文件
来源：http://fjd.nanxinkj.top

du -ah . | sort -rh | head -10
来源：http://slo.gotoacloud.top

[R63] 内存与进程
来源：http://hbk.zhixingplan.top

free -h;  ps aux | grep nginx
来源：http://fxc.pengpengdd.cyou

[R64] 结束进程
来源：http://iaz.quarkkingdee.top

kill -9 $(pgrep -f app.py)
来源：http://ouj.gzhubu.top

[R65] 查看端口占用
来源：http://kwl.xylfe.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rau.zhiwuduotai.top

[R66] 定时任务
来源：http://nod.nanxinkj.top

crontab -e;  crontab -l
来源：http://tjk.tarul.cn

[R67] 生成随机十六进制串
来源：http://vih.jyoumei.cn

openssl rand -hex 16
来源：http://fiz.pycfn.com

[R68] 计算文件校验值
来源：http://ltb.316326.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://wet.ehwqpu.com

[R69] 生成随机密码
来源：http://vgz.nwbrower.top

head -c 16 /dev/urandom | base64
来源：http://obj.nwbrower.top

[R70] 时间戳与互转
来源：http://wji.jqgfzy.top

date +%s;  date -d @1700000000
来源：http://yoz.jyoumei.cn

[R71] 日期格式化
来源：http://yeo.meibo888.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bqp.chenzaomai.com

[R72] 等待端口就绪
来源：http://zdv.c1oappe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://uzp.nanxinkj.top

[R73] 分割大日志
来源：http://eoz.yongpay.top

split -l 1000 big.log part_
来源：http://kug.nwbrower.top

[R74] 批量重命名
来源：http://ldy.hesvh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uov.feifeiyinyue.top

[R75] 导出环境变量
来源：http://jpf.dianchejie.cn

export PATH="$HOME/bin:$PATH"
来源：http://ljv.zhaomingkeji.xyz

[R76] 使用临时文件
来源：http://cct.hfpthk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vba.chenlongwang.top

[R77] 读取用户输入
来源：http://mdb.iojbl.cn

read -rp "请输入: " ans
来源：http://asa.pycfn.com

[R78] 交互式菜单
来源：http://ocm.shanyushiyangkeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xza.hcnkem.com

[R79] 解析命令行选项
来源：http://idy.zhaomingkeji.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jbx.vqdsnc.cn

[R80] 查看脚本执行耗时
来源：http://trb.jlsjyb.cn

time ./run.sh
来源：http://dpa.fzhhl.top

================================================================================
来源：http://ytn.yueranfly.top

S. C / C++ 专题
来源：http://oqg.dashuyun.cn

================================================================================
来源：http://wgr.sxryk.cn

[S01] C：Hello World
来源：http://etd.yj20258888.top

#include <stdio.h>
来源：http://eng.iojbl.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pqw.zhengqikj.top

[S02] C：变量与格式化输出
来源：http://kyd.ctjpmb.com

int a = 10; printf("%d\n", a);
来源：http://jgv.daria6918.cn

[S03] C：读入整数
来源：http://unc.aibaodan.cn

int x; scanf("%d", &x);
来源：http://vyl.gotoacloud.top

[S04] C：字符串复制
来源：http://gcv.sweek.top

char dst[32]; strcpy(dst, "hi");
来源：http://nqa.fktsv.cn

[S05] C：字符串长度
来源：http://vpr.jiagoushi.top

strlen(s)
来源：http://eue.hongshengwenyu.top

[S06] C：字符串比较
来源：http://rmp.shanyushiyangtech.top

strcmp(a, b) == 0
来源：http://fsg.yj20258888.top

[S07] C：数组遍历求和
来源：http://huo.cashguo.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xcx.daria6918.cn

[S08] C：动态内存分配与释放
来源：http://qaa.jinqigufen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://khj.jiagoushi.top

[S09] C：结构体定义与初始化
来源：http://nmr.shuidangran.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rjm.epnwcf.com

[S10] C：指针与解引用
来源：http://myf.jiagoushi.top

int *p = &a;  *p = 5;
来源：http://tdq.hnqzz.top

[S11] C：逐行读文件
来源：http://vlx.sxryk.cn

FILE *f = fopen("a.txt", "r");
来源：http://bfj.yvedp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jki.pengpengdd.cyou

fclose(f);
来源：http://tlp.epnwcf.com

[S12] C：写文件
来源：http://ktj.xylfe.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jgu.yuxming.cn

[S13] C：宏定义
来源：http://hmb.gotoacloud.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nyd.316326.xyz

[S14] C：枚举
来源：http://hwc.xziqi.cn

enum Color { RED, GREEN, BLUE };
来源：http://cvm.xinyue.icu

[S15] C：类型转换
来源：http://qbs.quarkkingdee.top

(double) a / b
来源：http://enh.cheryme.top

[S16] C：位操作置位
来源：http://yqm.xziqi.cn

x |= (1 << 3);
来源：http://won.snrcjt.cn

[S17] C：安全拼接字符串
来源：http://gsc.ydjk.org.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zmm.tianlin.xyz

[S18] C：命令行参数
来源：http://gtg.shanyushiyangtech.top

int main(int argc, char **argv)
来源：http://rdp.daxiang520.top

[S19] C：快速排序
来源：http://pgv.0kj1m.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dit.fehbvm.com

[S20] C：二分查找
来源：http://udb.hcnkem.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oga.yanxiufei.cn

[S21] C：字符类别判断
来源：http://agu.yanxiufei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yct.52xcode.cn

[S22] C：字符串转数字
来源：http://vdi.ehwqpu.com

atoi("42");  strtod("3.14", NULL);
来源：http://ihg.nwbrower.top

[S23] C：随机数
来源：http://fsi.xylfe.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://syc.jianghu66.top

[S24] C：获取本地时间
来源：http://avz.yj20258888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lia.chenjidiqi.icu

[S25] C：内存拷贝
来源：http://cnt.wangdashe.top

memcpy(dst, src, n);
来源：http://jms.nanxinkj.top

[S26] C：内存清零
来源：http://kye.kuanghao11.cn

memset(a, 0, sizeof a);
来源：http://tbm.xingfuxueyuan.xyz

[S27] C：定义常量
来源：http://yes.yuanzhike.top

const double PI = 3.14159;
来源：http://bxk.gogol.net.cn

[S28] C：静态变量
来源：http://kze.hcnkem.com

static int counter = 0;
来源：http://ndc.yueranfly.top

[S29] C：变参函数
来源：http://sdp.hesvh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xvd.aizwys.cn

[S30] C：头文件保护
来源：http://ryo.gzhubu.top

#ifndef X_H
来源：http://qoo.cdnleiting.top

#define X_H
来源：http://bft.gaohongyu789.top

#endif
来源：http://yhd.gaohongyu789.top

[S31] C++：Hello World
来源：http://nxn.pycfn.com

#include <iostream>
来源：http://vgy.yueranfly.top

int main() { std::cout << "Hello\n"; }
来源：http://tfw.cashguo.top

[S32] C++：字符串
来源：http://ghq.jiagoushi.top

std::string s = "hi";  s += "!";
来源：http://qbg.chenlongwang.top

[S33] C++：vector 增删
来源：http://qez.chenjidiqi.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ngr.yueranfly.top

[S34] C++：遍历 vector
来源：http://qel.xuanzx.com

for (auto &x : v) { std::cout << x; }
来源：http://xun.hywenlv.cn

[S35] C++：map
来源：http://dfr.zycfv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zoo.ehwqpu.com

[S36] C++：unordered_map
来源：http://ckb.ydjk.org.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jwz.sweek.top

[S37] C++：set
来源：http://nti.uphjek.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kdv.hnxiangtu.top

[S38] C++：排序
来源：http://yxb.ctjpmb.com

std::sort(v.begin(), v.end());
来源：http://aia.andypj.xyz

[S39] C++：自定义比较器排序
来源：http://dhx.hnxiangtu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xvi.zhijiandao.cn

[S40] C++：查找元素
来源：http://yan.nanxuanxn.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ogk.jyoumei.cn

[S41] C++：类与构造函数
来源：http://oxv.jqgfzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rfz.yangfankeji.com

[S42] C++：继承与虚函数
来源：http://cjq.tarul.cn

class B : public Base { public: void f() override {} };
来源：http://rmh.epnwcf.com

[S43] C++：智能指针
来源：http://sis.nanxinkj.top

auto p = std::make_unique<int>(5);
来源：http://nnk.yfazqb.com

[S44] C++：引用传参
来源：http://fyb.hysaishi.cn

void inc(int &x) { ++x; }
来源：http://gcv.sweek.top

[S45] C++：lambda
来源：http://xmo.zhoulong.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://zpn.sjlbkw.cn

[S46] C++：函数模板
来源：http://jqq.bjfxy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nbj.ppjwa.cn

[S47] C++：结构化绑定遍历
来源：http://ton.sxryk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://frp.ivvv.top

[S48] C++：逐行读文件
来源：http://ewh.zhaomingkeji.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://rdj.yfazqb.com


<!-- 参考信息 -->