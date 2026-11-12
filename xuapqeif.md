代发 wailian999

[Q76] 按天统计
来源：http://rox.daxiang520.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ocg.cucudq.cn

[Q77] 时间加减
来源：http://fvt.sxryk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tem.meibo888.top

[Q78] 当前时间
来源：http://rbw.0kj1m.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hxk.haohaochexian.top

[Q79] 字符串拼接
来源：http://cnl.hnqzz.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zaj.jinqigufen.top

[Q80] 字符串截取
来源：http://kwm.ydzc1.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gfc.sufxvd.cn

[Q81] 字符串替换
来源：http://iqx.tanke756.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://asg.shanyushiyangkeji.top

[Q82] 字符长度与字节长度
来源：http://gpv.shuidangran.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jhw.daria6918.cn

[Q83] 大小写转换
来源：http://khv.bbcook.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rkb.jinyuanbaomall.cn

[Q84] 去除首尾空格
来源：http://gbh.cashguo.top

SELECT TRIM(name) FROM users;
来源：http://grr.xuetiantiany.cn

[Q85] 数值取整
来源：http://ygy.yongpay.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cnc.jinqigfzy.top

[Q86] 读取 JSON 字段
来源：http://mqj.zhijiandao.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uyq.zycfv.cn

[Q87] JSON 字段做条件
来源：http://upv.mhx1999.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qnj.fehbvm.com

[Q88] 行转列（条件聚合）
来源：http://lpr.xuanzx.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lie.jiagoushi.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ljb.jlsjyb.cn

[Q89] 判断表是否存在
来源：http://mpe.jlsjyb.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hsd.ybcxt.top

[Q90] 生成序号列
来源：http://auq.hongshengwenyu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pqo.xylfe.cn

================================================================================
来源：http://svc.tian-w.cn

R. Bash 专题
来源：http://lnh.fktsv.cn

================================================================================
来源：http://esw.xuetiantiany.cn

[R01] shebang 与严格模式
来源：http://gwf.9152youxi.cn

#!/usr/bin/env bash
来源：http://eup.ywan-chungtsiang.top

set -euo pipefail
来源：http://ngw.jqgufenzy.top

[R02] 变量赋值与使用
来源：http://tei.dashuyun.cn

name="Tom"; echo "$name"
来源：http://aqs.nwbrower.top

[R03] 只读变量
来源：http://vac.gotoacloud.top

readonly PI=3.14
来源：http://dii.hammf.cn

[R04] 位置参数
来源：http://oeh.gogol.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gqs.nwbrower.top

[R05] 参数默认值
来源：http://gne.aizwys.cn

name="${1:-default}"
来源：http://ebs.bbcook.cn

[R06] 判断命令是否存在
来源：http://kmo.shangyingyoupin.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dra.redwolf501.top

[R07] if 判断文件
来源：http://umc.cqqwz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qtf.ppjwa.cn

[R08] 数值比较
来源：http://dnq.xuanzx.com

if (( a > b )); then echo "a 更大"; fi
来源：http://yfl.vqdsnc.cn

[R09] 字符串比较
来源：http://oex.sxryk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cfc.sjlbkw.cn

[R10] 正则匹配
来源：http://fah.gaohongyu789.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rkt.vehdjk.com

[R11] case 多分支
来源：http://aer.ctjpmb.com

case "$1" in
来源：http://uua.daxiang520.top

start) echo "启动" ;;
来源：http://uzt.shanyushiyangkeji.top

stop)  echo "停止" ;;
来源：http://aiu.zhoulong.xyz

*)     echo "未知命令" ;;
来源：http://ujo.cqqwz.cn

esac
来源：http://usu.nanxinkj.top

[R12] for 遍历文件
来源：http://yfw.chenzaomai.com

for f in *.txt; do echo "$f"; done
来源：http://pjl.pengpengdd.cyou

[R13] for 计数循环
来源：http://zqt.fanxiaobao.xyz

for i in {1..10}; do echo "$i"; done
来源：http://xap.tarul.cn

[R14] C 风格 for
来源：http://eqe.tanke756.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mgi.kuanghao11.cn

[R15] while 逐行读文件
来源：http://pju.ehwqpu.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lsh.xziqi.cn

[R16] until 等待条件
来源：http://tpi.jinyuanbaomall.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://chd.redwolf501.top

[R17] 数组定义与取值
来源：http://ujs.cashguo.top

arr=(a b c); echo "${arr[0]}"
来源：http://iqd.shuidangran.top

[R18] 遍历数组
来源：http://ezx.meibo888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gri.havefunace.top

[R19] 数组长度
来源：http://rkg.hcnkem.com

echo "${#arr[@]}"
来源：http://zgx.cdnleiting.top

[R20] 关联数组（字典）
来源：http://dvz.xylfe.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oqt.ehwqpu.com

[R21] 字符串长度
来源：http://pkd.sufxvd.cn

echo "${#s}"
来源：http://ele.zhijiandao.cn

[R22] 截取子串
来源：http://hmt.havefunace.top

echo "${s:0:5}"
来源：http://egj.dianchejie.cn

[R23] 字符串替换
来源：http://jwb.hfpthk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yue.9152youxi.cn

[R24] 大小写转换
来源：http://rfx.jqgufenzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://hty.zhijiandao.cn

[R25] 去后缀 / 去前缀
来源：http://ehy.0kj1m.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://grl.nanxinkj.top

[R26] 命令替换
来源：http://iai.xuetiantiany.cn

now=$(date +%F); echo "$now"
来源：http://ksm.tianlin.xyz

[R27] 算术展开
来源：http://bha.feifeiyinyue.top

echo $((1 + 2 * 3))
来源：http://wfl.smart0.xyz

[R28] 浮点运算
来源：http://zku.jinqigfzy.top

echo "scale=2; 10/3" | bc
来源：http://lwj.yvedp.cn

[R29] 定义函数
来源：http://gpo.fehbvm.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nee.zhaomingkeji.xyz

[R30] 函数返回状态码
来源：http://ayz.yueranfly.top

f() { return 0; }; f || echo "失败了"
来源：http://efm.mhx1999.top

[R31] 局部变量
来源：http://ifh.pycfn.com

f() { local x=1; echo "$x"; }
来源：http://ulu.c1oappe.top

[R32] 参数个数校验
来源：http://esn.zdbjq.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mcr.feifeiyinyue.top

[R33] 捕获错误并提示行号
来源：http://uqw.nwbrower.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://drb.tian-w.cn

[R34] 退出时清理
来源：http://opx.ybcxt.top

trap 'rm -f "$tmp"' EXIT
来源：http://fsr.gotoacloud.top

[R35] 后台执行并等待
来源：http://vwi.feifeiyinyue.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hlo.cdnleiting.top

[R36] 并发执行多个任务
来源：http://zod.uphjek.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rty.c1oappe.top

[R37] 把输出赋给变量
来源：http://rxs.nanxuanxn.top

files=$(ls -1)
来源：http://dfn.gotoacloud.top

[R38] 管道串联
来源：http://wlh.shuidangran.top

cat a.txt | grep -i error | wc -l
来源：http://uxa.hnxiangtu.top

[R39] 重定向标准输出与错误
来源：http://dez.mhx1999.top

cmd > out.log 2>&1
来源：http://vmo.shangyingyoupin.top

[R40] 追加写日志
来源：http://ggr.cashguo.top

echo "log" >> out.log
来源：http://fhb.hysaishi.cn

[R41] 丢弃输出
来源：http://mdj.guowangkeji.top

cmd >/dev/null 2>&1
来源：http://dgg.316326.xyz

[R42] 输入重定向
来源：http://ecu.jqgufenzy.top

wc -l < a.txt
来源：http://fnj.meibo888.top

[R43] 按名字查找文件
来源：http://rfv.hesvh.cn

find . -name "*.log" -type f
来源：http://zei.yangfankeji.com

[R44] 按修改时间查找
来源：http://lit.havefunace.top

find . -mtime -7 -type f
来源：http://zov.gzhubu.top

[R45] 批量删除
来源：http://grh.zhongyouzk.top

find . -name "*.tmp" -delete
来源：http://ght.quarkkingdee.top

[R46] 递归替换文件内容
来源：http://bno.tanke756.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bgo.zdbjq.cn

[R47] sed 单行替换
来源：http://koh.kuanghao11.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lpm.ppjwa.cn

[R48] awk 取指定列
来源：http://rbc.chenjidiqi.icu

awk '{print $1, $3}' a.txt
来源：http://hqu.zhaomingkeji.xyz

[R49] awk 带条件
来源：http://zej.vqdsnc.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://for.yongpay.top

[R50] awk 求和
来源：http://uuh.yueranfly.top

awk '{s += $2} END {print s}' a.txt
来源：http://tyy.ivvv.top

[R51] 排序去重取前几
来源：http://hty.cashguo.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rsk.uphjek.com

[R52] 统计行数
来源：http://ltm.shzxlz.cn

wc -l a.txt
来源：http://pul.ybcxt.top

[R53] 查看文件头与实时尾
来源：http://dtc.cdnleiting.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qkx.zycfv.cn

[R54] 比较两个文件
来源：http://ifa.quarkkingdee.top

diff a.txt b.txt
来源：http://oxx.sufxvd.cn

[R55] 压缩与解压
来源：http://buk.316326.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vxn.epnwcf.com

[R56] 远程拷贝
来源：http://mcr.shanyushiyangkeji.top

scp file user@host:/path/
来源：http://jvy.ivvv.top

[R57] 远程执行命令
来源：http://tyg.dianchejie.cn

ssh user@host 'uptime'
来源：http://eul.ybcxt.top

[R58] 下载文件
来源：http://ert.dashuyun.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bpj.sysykeji.top

[R59] 发 POST JSON
来源：http://fvs.chenlongwang.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zet.hnqzz.top

[R60] 只看 HTTP 状态码
来源：http://itn.jinghuilouyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rem.feifeiyinyue.top

[R61] 磁盘占用
来源：http://psm.redwolf501.top

df -h;  du -sh *
来源：http://rsu.sysykeji.top

[R62] 找最占空间的文件
来源：http://trc.iojbl.cn

du -ah . | sort -rh | head -10
来源：http://tar.zdqjudy.top

[R63] 内存与进程
来源：http://fyy.birdmap.top

free -h;  ps aux | grep nginx
来源：http://coh.fktsv.cn

[R64] 结束进程
来源：http://qrw.hcnkem.com

kill -9 $(pgrep -f app.py)
来源：http://shq.jinyuanbaomall.cn

[R65] 查看端口占用
来源：http://fqf.zhengqikj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oqq.hongshengwenyu.top

[R66] 定时任务
来源：http://dea.9152youxi.cn

crontab -e;  crontab -l
来源：http://ghr.jianghu66.top

[R67] 生成随机十六进制串
来源：http://pcr.fktsv.cn

openssl rand -hex 16
来源：http://htm.aizwys.cn

[R68] 计算文件校验值
来源：http://afc.c1oappe.top

sha256sum a.txt;  md5sum a.txt
来源：http://uea.sufxvd.cn

[R69] 生成随机密码
来源：http://yob.zhongyouzk.top

head -c 16 /dev/urandom | base64
来源：http://xyh.jqgufenzy.top

[R70] 时间戳与互转
来源：http://hdy.ctjpmb.com

date +%s;  date -d @1700000000
来源：http://kmr.wangshuangyany.cn

[R71] 日期格式化
来源：http://oix.zhaomingkeji.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://ang.xuetiantiany.cn

[R72] 等待端口就绪
来源：http://aln.hfpthk.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qkf.hesvh.cn

[R73] 分割大日志
来源：http://txv.nanxuanxn.top

split -l 1000 big.log part_
来源：http://pzt.tian-w.cn

[R74] 批量重命名
来源：http://uko.ywan-chungtsiang.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lcl.jqgufenzy.top

[R75] 导出环境变量
来源：http://oxo.daria6918.cn

export PATH="$HOME/bin:$PATH"
来源：http://pmz.chenlongwang.top

[R76] 使用临时文件
来源：http://wad.meibo888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nti.dashuyun.cn

[R77] 读取用户输入
来源：http://ile.zhaomingkeji.xyz

read -rp "请输入: " ans
来源：http://yrj.andypj.xyz

[R78] 交互式菜单
来源：http://azg.aizwys.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rbz.gogol.net.cn

[R79] 解析命令行选项
来源：http://usg.zycfv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://olw.9152youxi.cn

[R80] 查看脚本执行耗时
来源：http://nbo.guannengcc.top

time ./run.sh
来源：http://okp.zhoulong.xyz

================================================================================
来源：http://ymq.tian-w.cn

S. C / C++ 专题
来源：http://dls.zhoulong.xyz

================================================================================
来源：http://rtj.zhixingplan.top

[S01] C：Hello World
来源：http://kaa.ivvv.top

#include <stdio.h>
来源：http://rat.chenzaomai.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://uan.meibo888.top

[S02] C：变量与格式化输出
来源：http://rfd.yj202588.top

int a = 10; printf("%d\n", a);
来源：http://thz.jinqigufen.top

[S03] C：读入整数
来源：http://gyr.dianchejie.cn

int x; scanf("%d", &x);
来源：http://hmr.gaohongyu789.top

[S04] C：字符串复制
来源：http://fro.epnwcf.com

char dst[32]; strcpy(dst, "hi");
来源：http://guv.havefunace.top

[S05] C：字符串长度
来源：http://lde.xuetiantiany.cn

strlen(s)
来源：http://qou.yvedp.cn

[S06] C：字符串比较
来源：http://oss.xuanzx.com

strcmp(a, b) == 0
来源：http://mex.cashguo.top

[S07] C：数组遍历求和
来源：http://dqk.bjfxy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jok.sxryk.cn

[S08] C：动态内存分配与释放
来源：http://vnt.ybcxt.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zcn.tanke756.top

[S09] C：结构体定义与初始化
来源：http://khw.nanxinkj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lgf.ywan-chungtsiang.top

[S10] C：指针与解引用
来源：http://vlk.aibaodan.cn

int *p = &a;  *p = 5;
来源：http://vrb.cheryme.top

[S11] C：逐行读文件
来源：http://yrj.aibaodan.cn

FILE *f = fopen("a.txt", "r");
来源：http://lqt.hnqzz.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ogc.chenlongwang.top

fclose(f);
来源：http://sut.tian-w.cn

[S12] C：写文件
来源：http://ftu.svipenyu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qnb.zhoulong.xyz

[S13] C：宏定义
来源：http://kue.nanxuanxn.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pbt.chenlongwang.top

[S14] C：枚举
来源：http://dve.hesvh.cn

enum Color { RED, GREEN, BLUE };
来源：http://uty.gogol.net.cn

[S15] C：类型转换
来源：http://ngs.wangdashe.top

(double) a / b
来源：http://uev.meibo888.top

[S16] C：位操作置位
来源：http://kbf.chenlongwang.top

x |= (1 << 3);
来源：http://xll.yvedp.cn

[S17] C：安全拼接字符串
来源：http://lwr.yonumen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dbf.cqqwz.cn

[S18] C：命令行参数
来源：http://mto.yonumen.top

int main(int argc, char **argv)
来源：http://jko.jinqigufen.top

[S19] C：快速排序
来源：http://zjv.quarkkingdee.top

qsort(a, n, sizeof(int), cmp);
来源：http://tbf.xinyue.icu

[S20] C：二分查找
来源：http://hsa.hammf.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vvx.yvedp.cn

[S21] C：字符类别判断
来源：http://lgc.jinghuilouyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fuo.hfpthk.cn

[S22] C：字符串转数字
来源：http://omj.ehwqpu.com

atoi("42");  strtod("3.14", NULL);
来源：http://gmj.nanxinkj.top

[S23] C：随机数
来源：http://tqk.daria6918.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bzm.dianchejie.cn

[S24] C：获取本地时间
来源：http://hmc.hongshengwenyu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://djt.nanxinkj.top

[S25] C：内存拷贝
来源：http://oar.0kj1m.cn

memcpy(dst, src, n);
来源：http://hbh.xuanzx.com

[S26] C：内存清零
来源：http://fem.yvedp.cn

memset(a, 0, sizeof a);
来源：http://ggd.jlsjyb.cn

[S27] C：定义常量
来源：http://hph.guowangkeji.top

const double PI = 3.14159;
来源：http://ihf.guowangkeji.top

[S28] C：静态变量
来源：http://tkd.zdbjq.cn

static int counter = 0;
来源：http://dyp.xingfuxueyuan.xyz

[S29] C：变参函数
来源：http://gle.meibo888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ncn.zhiwuduotai.top

[S30] C：头文件保护
来源：http://fyj.meibo888.top

#ifndef X_H
来源：http://fta.zhengqikj.top

#define X_H
来源：http://jtk.yuanzhike.top

#endif
来源：http://quf.quarkkingdee.top

[S31] C++：Hello World
来源：http://sbb.vehdjk.com

#include <iostream>
来源：http://lzu.aibaodan.cn

int main() { std::cout << "Hello\n"; }
来源：http://mzv.yj202588.top

[S32] C++：字符串
来源：http://wxi.jinqigfzy.top

std::string s = "hi";  s += "!";
来源：http://aqn.fzhhl.top

[S33] C++：vector 增删
来源：http://fvk.52xcode.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sum.guowangkeji.top

[S34] C++：遍历 vector
来源：http://apq.epnwcf.com

for (auto &x : v) { std::cout << x; }
来源：http://bqw.wangdashe.top

[S35] C++：map
来源：http://sua.yfazqb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ksm.yj202588.top

[S36] C++：unordered_map
来源：http://lvj.yuxming.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sfg.meibo888.top

[S37] C++：set
来源：http://ole.daria6918.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xdf.jinyuanbaomall.cn

[S38] C++：排序
来源：http://meg.zhiwuduotai.top

std::sort(v.begin(), v.end());
来源：http://inu.yfazqb.com

[S39] C++：自定义比较器排序
来源：http://lox.yueranfly.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xmb.zdbjq.cn

[S40] C++：查找元素
来源：http://kux.zhaomingkeji.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tan.wangshuangyany.cn

[S41] C++：类与构造函数
来源：http://fhg.snrcjt.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sye.zdbjq.cn

[S42] C++：继承与虚函数
来源：http://hqv.hcnkem.com

class B : public Base { public: void f() override {} };
来源：http://jyg.ehwqpu.com

[S43] C++：智能指针
来源：http://bts.chenjidiqi.icu

auto p = std::make_unique<int>(5);
来源：http://skg.yueranfly.top

[S44] C++：引用传参
来源：http://vpd.wangdashe.top

void inc(int &x) { ++x; }
来源：http://gfp.bbcook.cn

[S45] C++：lambda
来源：http://cll.ywan-chungtsiang.top

auto add = [](int a, int b) { return a + b; };
来源：http://rgc.zdbjq.cn

[S46] C++：函数模板
来源：http://vjb.cashguo.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jrg.hfpthk.cn


<!-- 参考信息 -->