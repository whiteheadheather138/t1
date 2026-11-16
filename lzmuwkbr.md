代发 wailian999

ROLLBACK TO sp1;
来源：http://bur.yj20258888.top

[Q69] 查看执行计划
来源：http://zrn.dianchejie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ujl.chenzaomai.com

[Q70] 更新统计信息
来源：http://syz.xuetiantiany.cn

ANALYZE TABLE users;
来源：http://wvc.aizwys.cn

[Q71] 查看建表语句
来源：http://xum.shanyushiyangtech.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zxg.svipenyu.cn

[Q72] 查看索引
来源：http://hoj.hammf.cn

SHOW INDEX FROM users;
来源：http://ngi.hysaishi.cn

[Q73] 查看表状态
来源：http://ljp.fktsv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kky.dashuyun.cn

[Q74] 强制使用索引
来源：http://xav.snrcjt.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uoe.cdnleiting.top

[Q75] 日期格式化
来源：http://cqi.yuanzhike.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://avj.sweek.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oxt.snrcjt.cn

[Q76] 按天统计
来源：http://apc.yanxiufei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jgm.zhoulong.xyz

[Q77] 时间加减
来源：http://hmm.shanyushiyangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yll.ppjwa.cn

[Q78] 当前时间
来源：http://yqs.tian-w.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ifa.guowangkeji.top

[Q79] 字符串拼接
来源：http://yxf.yongpay.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nud.shangyingyoupin.top

[Q80] 字符串截取
来源：http://iyf.xuanzx.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://suq.zhengqikj.top

[Q81] 字符串替换
来源：http://lfe.hnxiangtu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jjw.sysykeji.top

[Q82] 字符长度与字节长度
来源：http://nob.nanxinkj.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uap.fengsongda.top

[Q83] 大小写转换
来源：http://huy.zycfv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://iop.ctjpmb.com

[Q84] 去除首尾空格
来源：http://ujz.yueranfly.top

SELECT TRIM(name) FROM users;
来源：http://krd.fzhhl.top

[Q85] 数值取整
来源：http://rwx.iojbl.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nst.svipenyu.cn

[Q86] 读取 JSON 字段
来源：http://kdf.xuanzx.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://swx.tianlin.xyz

[Q87] JSON 字段做条件
来源：http://sve.iojbl.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ymp.chenlongwang.top

[Q88] 行转列（条件聚合）
来源：http://csd.tarul.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tyc.yj20258.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gzj.cheryme.top

[Q89] 判断表是否存在
来源：http://duu.gotoacloud.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jzs.hnqzz.top

[Q90] 生成序号列
来源：http://kdg.andypj.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xyl.daria6918.cn

================================================================================
来源：http://iwi.jinqigfzy.top

R. Bash 专题
来源：http://xng.jlsjyb.cn

================================================================================
来源：http://flm.chenjidiqi.icu

[R01] shebang 与严格模式
来源：http://jia.jiagoushi.top

#!/usr/bin/env bash
来源：http://mmv.smart0.xyz

set -euo pipefail
来源：http://cdu.jinyuanbaomall.cn

[R02] 变量赋值与使用
来源：http://doz.aizwys.cn

name="Tom"; echo "$name"
来源：http://kpg.birdmap.top

[R03] 只读变量
来源：http://jwc.jyoumei.cn

readonly PI=3.14
来源：http://uzq.daxiang520.top

[R04] 位置参数
来源：http://que.ybcxt.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pds.yj20258888.top

[R05] 参数默认值
来源：http://adk.yuanzhike.top

name="${1:-default}"
来源：http://uee.zdqjudy.top

[R06] 判断命令是否存在
来源：http://oqt.xinyue.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://aqb.316326.xyz

[R07] if 判断文件
来源：http://sqs.vqdsnc.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kzm.yj20258.top

[R08] 数值比较
来源：http://qti.ydjk.org.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dto.aizwys.cn

[R09] 字符串比较
来源：http://exb.0kj1m.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mtc.yanxiufei.cn

[R10] 正则匹配
来源：http://gbu.kuanghao11.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tbq.yfazqb.com

[R11] case 多分支
来源：http://zra.jqgfzy.top

case "$1" in
来源：http://jev.ywan-chungtsiang.top

start) echo "启动" ;;
来源：http://kok.dashuyun.cn

stop)  echo "停止" ;;
来源：http://zti.kuanghao11.cn

*)     echo "未知命令" ;;
来源：http://ssv.yuanzhike.top

esac
来源：http://gmj.zhiwuduotai.top

[R12] for 遍历文件
来源：http://mtc.zhongyouzk.top

for f in *.txt; do echo "$f"; done
来源：http://tew.fktsv.cn

[R13] for 计数循环
来源：http://utf.sysykeji.top

for i in {1..10}; do echo "$i"; done
来源：http://loz.vehdjk.com

[R14] C 风格 for
来源：http://fbn.ehwqpu.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ica.dianchejie.cn

[R15] while 逐行读文件
来源：http://nrn.zdqjudy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://njy.jqgufenzy.top

[R16] until 等待条件
来源：http://ffb.xuetiantiany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://esc.jianghu66.top

[R17] 数组定义与取值
来源：http://wnh.jinghuilouyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hgx.ybcxt.top

[R18] 遍历数组
来源：http://gzz.xylfe.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kwe.wangshuangyany.cn

[R19] 数组长度
来源：http://htz.zycfv.cn

echo "${#arr[@]}"
来源：http://qte.dianchejie.cn

[R20] 关联数组（字典）
来源：http://val.chenjidiqi.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://urj.guowangkeji.top

[R21] 字符串长度
来源：http://jep.nwbrower.top

echo "${#s}"
来源：http://ndx.hcnkem.com

[R22] 截取子串
来源：http://xfy.zhongyouzk.top

echo "${s:0:5}"
来源：http://atx.pengpengdd.cyou

[R23] 字符串替换
来源：http://tpk.yuxming.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kso.hesvh.cn

[R24] 大小写转换
来源：http://suk.xingfuxueyuan.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://qqi.0kj1m.cn

[R25] 去后缀 / 去前缀
来源：http://fcf.hcnkem.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://iez.birdmap.top

[R26] 命令替换
来源：http://ncr.pycfn.com

now=$(date +%F); echo "$now"
来源：http://khc.gaohongyu789.top

[R27] 算术展开
来源：http://fha.smart0.xyz

echo $((1 + 2 * 3))
来源：http://nhw.tanke756.top

[R28] 浮点运算
来源：http://wbu.gogol.net.cn

echo "scale=2; 10/3" | bc
来源：http://gud.yanxiufei.cn

[R29] 定义函数
来源：http://heg.hammf.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fbk.hnxiangtu.top

[R30] 函数返回状态码
来源：http://spt.316326.xyz

f() { return 0; }; f || echo "失败了"
来源：http://ymk.haohaochexian.top

[R31] 局部变量
来源：http://oay.chenlongwang.top

f() { local x=1; echo "$x"; }
来源：http://cyi.jiagoushi.top

[R32] 参数个数校验
来源：http://fsq.bbcook.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ocj.zdqjudy.top

[R33] 捕获错误并提示行号
来源：http://dgl.aizwys.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://prg.dianchejie.cn

[R34] 退出时清理
来源：http://bxt.vqdsnc.cn

trap 'rm -f "$tmp"' EXIT
来源：http://iod.jinqigfzy.top

[R35] 后台执行并等待
来源：http://zvw.ydzc1.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ndu.cheryme.top

[R36] 并发执行多个任务
来源：http://fbv.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ghu.ydzc1.top

[R37] 把输出赋给变量
来源：http://nig.sweek.top

files=$(ls -1)
来源：http://wsb.vqdsnc.cn

[R38] 管道串联
来源：http://xda.meibo888.top

cat a.txt | grep -i error | wc -l
来源：http://izn.redwolf501.top

[R39] 重定向标准输出与错误
来源：http://tua.shzxlz.cn

cmd > out.log 2>&1
来源：http://ssk.zhaomingkeji.xyz

[R40] 追加写日志
来源：http://aje.jinqigfzy.top

echo "log" >> out.log
来源：http://ggi.guannengcc.top

[R41] 丢弃输出
来源：http://eiu.ybcxt.top

cmd >/dev/null 2>&1
来源：http://wrw.feifeiyinyue.top

[R42] 输入重定向
来源：http://odh.hysaishi.cn

wc -l < a.txt
来源：http://ave.fengsongda.top

[R43] 按名字查找文件
来源：http://kzn.kuanghao11.cn

find . -name "*.log" -type f
来源：http://jto.yueranfly.top

[R44] 按修改时间查找
来源：http://yeh.tarul.cn

find . -mtime -7 -type f
来源：http://jku.vehdjk.com

[R45] 批量删除
来源：http://lte.gaohongyu789.top

find . -name "*.tmp" -delete
来源：http://bdt.tarul.cn

[R46] 递归替换文件内容
来源：http://etl.sufxvd.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uim.jinqigfzy.top

[R47] sed 单行替换
来源：http://puu.hongshengwenyu.top

sed -i 's/foo/bar/g' a.txt
来源：http://zlw.yvedp.cn

[R48] awk 取指定列
来源：http://jzv.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://hgr.redwolf501.top

[R49] awk 带条件
来源：http://thq.uphjek.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xif.zdbjq.cn

[R50] awk 求和
来源：http://tdd.zdbjq.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bjg.yangfankeji.com

[R51] 排序去重取前几
来源：http://wai.redwolf501.top

sort a.txt | uniq -c | sort -rn | head
来源：http://oqc.tanke756.top

[R52] 统计行数
来源：http://ahb.yonumen.top

wc -l a.txt
来源：http://vpm.hfpthk.cn

[R53] 查看文件头与实时尾
来源：http://uxm.yangfankeji.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qyi.birdmap.top

[R54] 比较两个文件
来源：http://sqp.aibaodan.cn

diff a.txt b.txt
来源：http://icm.snrcjt.cn

[R55] 压缩与解压
来源：http://hjn.zhengqikj.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gya.yvedp.cn

[R56] 远程拷贝
来源：http://fsp.jinghuilouyu.cn

scp file user@host:/path/
来源：http://xug.zdbjq.cn

[R57] 远程执行命令
来源：http://rzv.svipenyu.cn

ssh user@host 'uptime'
来源：http://ysa.nanxuanxn.top

[R58] 下载文件
来源：http://nyg.cdnleiting.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lti.tanke756.top

[R59] 发 POST JSON
来源：http://vpe.hongshengwenyu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xoy.shanyushiyangkeji.top

[R60] 只看 HTTP 状态码
来源：http://nuo.fehbvm.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lux.cashguo.top

[R61] 磁盘占用
来源：http://nku.cqqwz.cn

df -h;  du -sh *
来源：http://bpn.bbcook.cn

[R62] 找最占空间的文件
来源：http://ztu.shzxlz.cn

du -ah . | sort -rh | head -10
来源：http://cuq.vqdsnc.cn

[R63] 内存与进程
来源：http://fbp.nwbrower.top

free -h;  ps aux | grep nginx
来源：http://hzg.fktsv.cn

[R64] 结束进程
来源：http://zbj.sxryk.cn

kill -9 $(pgrep -f app.py)
来源：http://fpv.ppjwa.cn

[R65] 查看端口占用
来源：http://cno.haohaochexian.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kdt.pycfn.com

[R66] 定时任务
来源：http://ide.jlsjyb.cn

crontab -e;  crontab -l
来源：http://ugv.yvedp.cn

[R67] 生成随机十六进制串
来源：http://xwa.jinqigufen.top

openssl rand -hex 16
来源：http://bpr.ppjwa.cn

[R68] 计算文件校验值
来源：http://ljr.ivvv.top

sha256sum a.txt;  md5sum a.txt
来源：http://gnz.hysaishi.cn

[R69] 生成随机密码
来源：http://rqj.hnxiangtu.top

head -c 16 /dev/urandom | base64
来源：http://hwv.zhengqikj.top

[R70] 时间戳与互转
来源：http://tif.epnwcf.com

date +%s;  date -d @1700000000
来源：http://zfk.fanxiaobao.xyz

[R71] 日期格式化
来源：http://sru.gaohongyu789.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://knx.gogol.net.cn

[R72] 等待端口就绪
来源：http://vmp.jianghu66.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lly.tian-w.cn

[R73] 分割大日志
来源：http://mgs.sysykeji.top

split -l 1000 big.log part_
来源：http://fbl.hongshengwenyu.top

[R74] 批量重命名
来源：http://vkc.zhengqikj.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oww.fehbvm.com

[R75] 导出环境变量
来源：http://qnm.redwolf501.top

export PATH="$HOME/bin:$PATH"
来源：http://dbj.shangyingyoupin.top

[R76] 使用临时文件
来源：http://kkt.sxryk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://npy.52xcode.cn

[R77] 读取用户输入
来源：http://ajm.aibaodan.cn

read -rp "请输入: " ans
来源：http://hhd.yvedp.cn

[R78] 交互式菜单
来源：http://bra.haohaochexian.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ceq.hysaishi.cn

[R79] 解析命令行选项
来源：http://jwm.gotoacloud.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ddb.iojbl.cn

[R80] 查看脚本执行耗时
来源：http://joq.yj20258888.top

time ./run.sh
来源：http://zpj.uphjek.com

================================================================================
来源：http://gix.cqqwz.cn

S. C / C++ 专题
来源：http://zvg.cucudq.cn

================================================================================
来源：http://zpk.chenzaomai.com

[S01] C：Hello World
来源：http://oea.iojbl.cn

#include <stdio.h>
来源：http://dfs.zhaomingkeji.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://fnl.mhx1999.top

[S02] C：变量与格式化输出
来源：http://ehr.hywenlv.cn

int a = 10; printf("%d\n", a);
来源：http://mah.yuanzhike.top

[S03] C：读入整数
来源：http://pst.yvedp.cn

int x; scanf("%d", &x);
来源：http://wdo.ydzc1.top

[S04] C：字符串复制
来源：http://svx.kuanghao11.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gmt.tian-w.cn

[S05] C：字符串长度
来源：http://kah.shanyushiyangtech.top

strlen(s)
来源：http://bvl.aizwys.cn

[S06] C：字符串比较
来源：http://qdx.zhijiandao.cn

strcmp(a, b) == 0
来源：http://rzl.fengsongda.top

[S07] C：数组遍历求和
来源：http://bwi.kuanghao11.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mrv.nanxinkj.top

[S08] C：动态内存分配与释放
来源：http://ezq.zhaomingkeji.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://app.vehdjk.com

[S09] C：结构体定义与初始化
来源：http://hkz.zhaomingkeji.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qqg.bjfxy.top

[S10] C：指针与解引用
来源：http://eab.smart0.xyz

int *p = &a;  *p = 5;
来源：http://fwj.aibaodan.cn

[S11] C：逐行读文件
来源：http://rte.yangfankeji.com

FILE *f = fopen("a.txt", "r");
来源：http://zfg.sweek.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zyx.yuxming.cn

fclose(f);
来源：http://xyj.zdbjq.cn

[S12] C：写文件
来源：http://ntl.nanxinkj.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://auu.cucudq.cn

[S13] C：宏定义
来源：http://eku.zycfv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://iev.bbcook.cn

[S14] C：枚举
来源：http://jvh.jinqigfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://muq.bjfxy.top

[S15] C：类型转换
来源：http://mdl.zhengqikj.top

(double) a / b
来源：http://csu.gaohongyu789.top

[S16] C：位操作置位
来源：http://gid.cqqwz.cn

x |= (1 << 3);
来源：http://oou.gaohongyu789.top

[S17] C：安全拼接字符串
来源：http://bxt.zhaomingkeji.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://iao.jinqigufen.top

[S18] C：命令行参数
来源：http://hqb.zhixingplan.top

int main(int argc, char **argv)
来源：http://fac.zhengqikj.top

[S19] C：快速排序
来源：http://nyy.jinqigfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://xqk.tian-w.cn

[S20] C：二分查找
来源：http://fir.uphjek.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rdl.yuanzhike.top

[S21] C：字符类别判断
来源：http://esg.yj202588.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ykk.tarul.cn

[S22] C：字符串转数字
来源：http://nxl.sjlbkw.cn

atoi("42");  strtod("3.14", NULL);
来源：http://iku.chenjidiqi.icu

[S23] C：随机数
来源：http://juu.ydzc1.top

srand(time(NULL));  int r = rand() % 100;
来源：http://oou.cheryme.top

[S24] C：获取本地时间
来源：http://rcj.tarul.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dmn.fengsongda.top

[S25] C：内存拷贝
来源：http://sat.jinghuilouyu.cn

memcpy(dst, src, n);
来源：http://owp.sxryk.cn

[S26] C：内存清零
来源：http://veh.svipenyu.cn

memset(a, 0, sizeof a);
来源：http://gpk.316326.xyz

[S27] C：定义常量
来源：http://dpi.iojbl.cn

const double PI = 3.14159;
来源：http://edg.yongpay.top

[S28] C：静态变量
来源：http://art.nanxinkj.top

static int counter = 0;
来源：http://abh.hnqzz.top

[S29] C：变参函数
来源：http://ler.jlsjyb.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tof.iojbl.cn

[S30] C：头文件保护
来源：http://uwb.jianghu66.top

#ifndef X_H
来源：http://hij.jinqigufen.top

#define X_H
来源：http://isq.tanke756.top

#endif
来源：http://lkr.fzhhl.top

[S31] C++：Hello World
来源：http://flx.zdbjq.cn

#include <iostream>
来源：http://uor.jqgufenzy.top

int main() { std::cout << "Hello\n"; }
来源：http://yhu.haohaochexian.top

[S32] C++：字符串
来源：http://mas.xziqi.cn

std::string s = "hi";  s += "!";
来源：http://pak.chenlongwang.top

[S33] C++：vector 增删
来源：http://est.cheryme.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hsz.svipenyu.cn

[S34] C++：遍历 vector
来源：http://vpj.zhiwuduotai.top

for (auto &x : v) { std::cout << x; }
来源：http://dkn.bbcook.cn

[S35] C++：map
来源：http://qbt.hfpthk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://itr.gaohongyu789.top

[S36] C++：unordered_map
来源：http://lge.wangshuangyany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qxg.yongpay.top

[S37] C++：set
来源：http://rxn.zhengqikj.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zxi.feifeiyinyue.top

[S38] C++：排序
来源：http://iub.cdnleiting.top

std::sort(v.begin(), v.end());
来源：http://fac.vehdjk.com


<!-- 参考信息 -->