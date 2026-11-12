代发 wailian999

[Q65] 回滚事务
来源：http://emd.bjfxy.top

ROLLBACK;
来源：http://bjd.shanyushiyangtech.top

[Q66] 行锁查询
来源：http://dli.hongshengwenyu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hyf.fengsongda.top

[Q67] 设置隔离级别
来源：http://ava.yvedp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://psb.gzhubu.top

[Q68] 保存点
来源：http://mlf.quarkkingdee.top

SAVEPOINT sp1;
来源：http://wjm.yj202588.top

ROLLBACK TO sp1;
来源：http://caf.yonumen.top

[Q69] 查看执行计划
来源：http://omt.epnwcf.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wmi.svipenyu.cn

[Q70] 更新统计信息
来源：http://xaf.andypj.xyz

ANALYZE TABLE users;
来源：http://urx.c1oappe.top

[Q71] 查看建表语句
来源：http://fna.zhijiandao.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kpo.9152youxi.cn

[Q72] 查看索引
来源：http://rwk.sysykeji.top

SHOW INDEX FROM users;
来源：http://bqg.pengpengdd.cyou

[Q73] 查看表状态
来源：http://thw.xylfe.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ehw.cucudq.cn

[Q74] 强制使用索引
来源：http://blp.yfazqb.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tin.pycfn.com

[Q75] 日期格式化
来源：http://wnd.zycfv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ggq.hnxiangtu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pnh.guannengcc.top

[Q76] 按天统计
来源：http://tho.mhx1999.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qyf.yuxming.cn

[Q77] 时间加减
来源：http://egh.daxiang520.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pwz.jinqigufen.top

[Q78] 当前时间
来源：http://vfw.svipenyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jev.epnwcf.com

[Q79] 字符串拼接
来源：http://ibd.ybcxt.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ydo.jqgfzy.top

[Q80] 字符串截取
来源：http://ary.vqdsnc.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tzf.sxryk.cn

[Q81] 字符串替换
来源：http://kub.chenjidiqi.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fhk.zhijiandao.cn

[Q82] 字符长度与字节长度
来源：http://cvb.feifeiyinyue.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uym.fengsongda.top

[Q83] 大小写转换
来源：http://ivr.sweek.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gcn.ybcxt.top

[Q84] 去除首尾空格
来源：http://ipu.c1oappe.top

SELECT TRIM(name) FROM users;
来源：http://gaf.hcnkem.com

[Q85] 数值取整
来源：http://zym.jinyuanbaomall.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nic.hnqzz.top

[Q86] 读取 JSON 字段
来源：http://qvd.zhijiandao.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://djb.chenzaomai.com

[Q87] JSON 字段做条件
来源：http://hsr.bbcook.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wpg.uphjek.com

[Q88] 行转列（条件聚合）
来源：http://nky.zhijiandao.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rgn.ybcxt.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fxn.kuanghao11.cn

[Q89] 判断表是否存在
来源：http://pee.aibaodan.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wad.guowangkeji.top

[Q90] 生成序号列
来源：http://sjw.shzxlz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dwf.andypj.xyz

================================================================================
来源：http://exq.zhongyouzk.top

R. Bash 专题
来源：http://lde.gotoacloud.top

================================================================================
来源：http://nkx.ydzc1.top

[R01] shebang 与严格模式
来源：http://eks.vqdsnc.cn

#!/usr/bin/env bash
来源：http://uxd.tarul.cn

set -euo pipefail
来源：http://inc.jianghu66.top

[R02] 变量赋值与使用
来源：http://zth.ppjwa.cn

name="Tom"; echo "$name"
来源：http://efp.dashuyun.cn

[R03] 只读变量
来源：http://rst.dianchejie.cn

readonly PI=3.14
来源：http://pra.hysaishi.cn

[R04] 位置参数
来源：http://plt.birdmap.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gaj.jinqigfzy.top

[R05] 参数默认值
来源：http://nky.redwolf501.top

name="${1:-default}"
来源：http://zrn.hammf.cn

[R06] 判断命令是否存在
来源：http://ryi.birdmap.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dvh.xuetiantiany.cn

[R07] if 判断文件
来源：http://fkh.haohaochexian.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rpa.daxiang520.top

[R08] 数值比较
来源：http://sqr.aibaodan.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gxh.c1oappe.top

[R09] 字符串比较
来源：http://ozq.ywan-chungtsiang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xhz.daxiang520.top

[R10] 正则匹配
来源：http://zdc.ivvv.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xql.hywenlv.cn

[R11] case 多分支
来源：http://oxr.sjlbkw.cn

case "$1" in
来源：http://jcc.havefunace.top

start) echo "启动" ;;
来源：http://igk.tarul.cn

stop)  echo "停止" ;;
来源：http://mxy.pengpengdd.cyou

*)     echo "未知命令" ;;
来源：http://gmb.zhaomingkeji.xyz

esac
来源：http://azk.shuidangran.top

[R12] for 遍历文件
来源：http://wsp.9152youxi.cn

for f in *.txt; do echo "$f"; done
来源：http://uvr.dashuyun.cn

[R13] for 计数循环
来源：http://xkd.nanxinkj.top

for i in {1..10}; do echo "$i"; done
来源：http://roh.vqdsnc.cn

[R14] C 风格 for
来源：http://mwj.tianlin.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eoe.uphjek.com

[R15] while 逐行读文件
来源：http://xos.jinghuilouyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yxv.xziqi.cn

[R16] until 等待条件
来源：http://wep.zhongyouzk.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lxp.tarul.cn

[R17] 数组定义与取值
来源：http://zbm.quarkkingdee.top

arr=(a b c); echo "${arr[0]}"
来源：http://mbz.chenlongwang.top

[R18] 遍历数组
来源：http://xsp.xuetiantiany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wsi.shzxlz.cn

[R19] 数组长度
来源：http://rxo.havefunace.top

echo "${#arr[@]}"
来源：http://iwu.yanxiufei.cn

[R20] 关联数组（字典）
来源：http://zhu.mhx1999.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lmw.hnqzz.top

[R21] 字符串长度
来源：http://fyb.jyoumei.cn

echo "${#s}"
来源：http://cjn.shuidangran.top

[R22] 截取子串
来源：http://htx.hfpthk.cn

echo "${s:0:5}"
来源：http://tpy.pycfn.com

[R23] 字符串替换
来源：http://csr.gogol.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rnq.xuanzx.com

[R24] 大小写转换
来源：http://cdu.xylfe.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lws.hnqzz.top

[R25] 去后缀 / 去前缀
来源：http://kpo.gogol.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wcj.jyoumei.cn

[R26] 命令替换
来源：http://wau.meibo888.top

now=$(date +%F); echo "$now"
来源：http://min.316326.xyz

[R27] 算术展开
来源：http://vhx.52xcode.cn

echo $((1 + 2 * 3))
来源：http://cud.chenzaomai.com

[R28] 浮点运算
来源：http://tlj.gogol.net.cn

echo "scale=2; 10/3" | bc
来源：http://hhl.sxryk.cn

[R29] 定义函数
来源：http://mxp.xziqi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jsd.haohaochexian.top

[R30] 函数返回状态码
来源：http://app.shanyushiyangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://hhd.zhoulong.xyz

[R31] 局部变量
来源：http://nah.vehdjk.com

f() { local x=1; echo "$x"; }
来源：http://wrp.yj202588.top

[R32] 参数个数校验
来源：http://iky.vehdjk.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dnu.fehbvm.com

[R33] 捕获错误并提示行号
来源：http://xqn.cqqwz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mbx.ybcxt.top

[R34] 退出时清理
来源：http://duz.quarkkingdee.top

trap 'rm -f "$tmp"' EXIT
来源：http://xcx.wangshuangyany.cn

[R35] 后台执行并等待
来源：http://jab.gogol.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nrh.cucudq.cn

[R36] 并发执行多个任务
来源：http://zyz.ywan-chungtsiang.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bbf.zhoulong.xyz

[R37] 把输出赋给变量
来源：http://opm.wangshuangyany.cn

files=$(ls -1)
来源：http://sto.uphjek.com

[R38] 管道串联
来源：http://xcy.yvedp.cn

cat a.txt | grep -i error | wc -l
来源：http://wjt.nwbrower.top

[R39] 重定向标准输出与错误
来源：http://ddl.zhoulong.xyz

cmd > out.log 2>&1
来源：http://tac.kuanghao11.cn

[R40] 追加写日志
来源：http://whf.daxiang520.top

echo "log" >> out.log
来源：http://eyf.nanxinkj.top

[R41] 丢弃输出
来源：http://xya.daria6918.cn

cmd >/dev/null 2>&1
来源：http://jrc.pengpengdd.cyou

[R42] 输入重定向
来源：http://cdh.bjfxy.top

wc -l < a.txt
来源：http://hwk.ehwqpu.com

[R43] 按名字查找文件
来源：http://bja.yj20258.top

find . -name "*.log" -type f
来源：http://cvw.52xcode.cn

[R44] 按修改时间查找
来源：http://vwz.fengsongda.top

find . -mtime -7 -type f
来源：http://rxo.mhx1999.top

[R45] 批量删除
来源：http://kwa.zdqjudy.top

find . -name "*.tmp" -delete
来源：http://bvg.snrcjt.cn

[R46] 递归替换文件内容
来源：http://vot.shangyingyoupin.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bst.yonumen.top

[R47] sed 单行替换
来源：http://mea.cashguo.top

sed -i 's/foo/bar/g' a.txt
来源：http://qut.yuxming.cn

[R48] awk 取指定列
来源：http://gvg.xinyue.icu

awk '{print $1, $3}' a.txt
来源：http://feb.jinyuanbaomall.cn

[R49] awk 带条件
来源：http://ush.zhiwuduotai.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tad.316326.xyz

[R50] awk 求和
来源：http://chm.jinqigufen.top

awk '{s += $2} END {print s}' a.txt
来源：http://vlg.jqgufenzy.top

[R51] 排序去重取前几
来源：http://fbc.sjlbkw.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qqn.redwolf501.top

[R52] 统计行数
来源：http://pqb.bjfxy.top

wc -l a.txt
来源：http://sud.kuanghao11.cn

[R53] 查看文件头与实时尾
来源：http://tdc.pycfn.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hgx.xziqi.cn

[R54] 比较两个文件
来源：http://gud.shanyushiyangtech.top

diff a.txt b.txt
来源：http://rkk.zdqjudy.top

[R55] 压缩与解压
来源：http://tmn.zhaomingkeji.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://squ.fehbvm.com

[R56] 远程拷贝
来源：http://aht.sweek.top

scp file user@host:/path/
来源：http://czi.vehdjk.com

[R57] 远程执行命令
来源：http://klj.gotoacloud.top

ssh user@host 'uptime'
来源：http://uai.ydjk.org.cn

[R58] 下载文件
来源：http://rij.c1oappe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fns.quarkkingdee.top

[R59] 发 POST JSON
来源：http://qzi.ehwqpu.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gak.pycfn.com

[R60] 只看 HTTP 状态码
来源：http://yqc.yongpay.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bue.kuanghao11.cn

[R61] 磁盘占用
来源：http://jnj.bbcook.cn

df -h;  du -sh *
来源：http://ybk.hongshengwenyu.top

[R62] 找最占空间的文件
来源：http://xox.gzhubu.top

du -ah . | sort -rh | head -10
来源：http://mfg.birdmap.top

[R63] 内存与进程
来源：http://pyy.iojbl.cn

free -h;  ps aux | grep nginx
来源：http://kpd.dianchejie.cn

[R64] 结束进程
来源：http://rum.xylfe.cn

kill -9 $(pgrep -f app.py)
来源：http://vze.zdbjq.cn

[R65] 查看端口占用
来源：http://dnh.sweek.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://euw.wangdashe.top

[R66] 定时任务
来源：http://ggc.bjfxy.top

crontab -e;  crontab -l
来源：http://xjz.ydzc1.top

[R67] 生成随机十六进制串
来源：http://qcs.epnwcf.com

openssl rand -hex 16
来源：http://bzn.iojbl.cn

[R68] 计算文件校验值
来源：http://kdr.zhijiandao.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vwv.shuidangran.top

[R69] 生成随机密码
来源：http://nxk.ehwqpu.com

head -c 16 /dev/urandom | base64
来源：http://nvg.sxryk.cn

[R70] 时间戳与互转
来源：http://lxx.zhijiandao.cn

date +%s;  date -d @1700000000
来源：http://jqq.cdnleiting.top

[R71] 日期格式化
来源：http://spr.feifeiyinyue.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://act.jqgfzy.top

[R72] 等待端口就绪
来源：http://xvz.xinyue.icu

until nc -z localhost 3306; do sleep 1; done
来源：http://jve.hesvh.cn

[R73] 分割大日志
来源：http://oys.aibaodan.cn

split -l 1000 big.log part_
来源：http://xve.yj202588.top

[R74] 批量重命名
来源：http://ebk.pengpengdd.cyou

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ylb.vehdjk.com

[R75] 导出环境变量
来源：http://yjc.gogol.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://xkm.sweek.top

[R76] 使用临时文件
来源：http://lkz.pycfn.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://znr.hywenlv.cn

[R77] 读取用户输入
来源：http://tzb.52xcode.cn

read -rp "请输入: " ans
来源：http://zqt.zdbjq.cn

[R78] 交互式菜单
来源：http://pbj.jinqigufen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hvu.yj20258.top

[R79] 解析命令行选项
来源：http://kut.shuidangran.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oao.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://phm.wangshuangyany.cn

time ./run.sh
来源：http://ixl.sufxvd.cn

================================================================================
来源：http://dgg.shzxlz.cn

S. C / C++ 专题
来源：http://del.jyoumei.cn

================================================================================
来源：http://bbx.nwbrower.top

[S01] C：Hello World
来源：http://hpl.havefunace.top

#include <stdio.h>
来源：http://mph.svipenyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ogq.9152youxi.cn

[S02] C：变量与格式化输出
来源：http://fda.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://deu.shangyingyoupin.top

[S03] C：读入整数
来源：http://nvh.hywenlv.cn

int x; scanf("%d", &x);
来源：http://lit.aizwys.cn

[S04] C：字符串复制
来源：http://guf.yfazqb.com

char dst[32]; strcpy(dst, "hi");
来源：http://oby.yonumen.top

[S05] C：字符串长度
来源：http://rqw.jinyuanbaomall.cn

strlen(s)
来源：http://xgr.yj20258.top

[S06] C：字符串比较
来源：http://ibq.tanke756.top

strcmp(a, b) == 0
来源：http://vyl.hysaishi.cn

[S07] C：数组遍历求和
来源：http://dbu.fehbvm.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gfl.sysykeji.top

[S08] C：动态内存分配与释放
来源：http://das.jiagoushi.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ruv.gotoacloud.top

[S09] C：结构体定义与初始化
来源：http://cwp.yongpay.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bhl.ybcxt.top

[S10] C：指针与解引用
来源：http://cgs.vehdjk.com

int *p = &a;  *p = 5;
来源：http://wvy.sufxvd.cn

[S11] C：逐行读文件
来源：http://dew.birdmap.top

FILE *f = fopen("a.txt", "r");
来源：http://ugs.zhixingplan.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://let.daxiang520.top

fclose(f);
来源：http://xmw.dianchejie.cn

[S12] C：写文件
来源：http://rwx.xuanzx.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pou.hesvh.cn

[S13] C：宏定义
来源：http://ban.sysykeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ivs.nanxuanxn.top

[S14] C：枚举
来源：http://klh.epnwcf.com

enum Color { RED, GREEN, BLUE };
来源：http://yiv.0kj1m.cn

[S15] C：类型转换
来源：http://ndw.cqqwz.cn

(double) a / b
来源：http://tou.quarkkingdee.top

[S16] C：位操作置位
来源：http://wti.cashguo.top

x |= (1 << 3);
来源：http://pkc.ydzc1.top

[S17] C：安全拼接字符串
来源：http://dmj.shangyingyoupin.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mcv.aibaodan.cn

[S18] C：命令行参数
来源：http://tic.yangfankeji.com

int main(int argc, char **argv)
来源：http://iho.nanxinkj.top

[S19] C：快速排序
来源：http://sxl.jiagoushi.top

qsort(a, n, sizeof(int), cmp);
来源：http://lis.yangfankeji.com

[S20] C：二分查找
来源：http://xit.9152youxi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gtl.ydjk.org.cn

[S21] C：字符类别判断
来源：http://rcg.uphjek.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bxb.kuanghao11.cn

[S22] C：字符串转数字
来源：http://qle.zdqjudy.top

atoi("42");  strtod("3.14", NULL);
来源：http://oqp.sweek.top

[S23] C：随机数
来源：http://kwt.tanke756.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hxe.hywenlv.cn

[S24] C：获取本地时间
来源：http://gyh.cdnleiting.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ntb.ctjpmb.com

[S25] C：内存拷贝
来源：http://sez.yonumen.top

memcpy(dst, src, n);
来源：http://edm.tanke756.top

[S26] C：内存清零
来源：http://vjc.tarul.cn

memset(a, 0, sizeof a);
来源：http://abu.jiagoushi.top

[S27] C：定义常量
来源：http://lyh.hesvh.cn

const double PI = 3.14159;
来源：http://mzw.andypj.xyz

[S28] C：静态变量
来源：http://whk.shanyushiyangtech.top

static int counter = 0;
来源：http://yho.fehbvm.com

[S29] C：变参函数
来源：http://jnd.nanxinkj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qct.redwolf501.top

[S30] C：头文件保护
来源：http://big.hnxiangtu.top

#ifndef X_H
来源：http://tcs.zhijiandao.cn

#define X_H
来源：http://ggg.316326.xyz

#endif
来源：http://vrj.fehbvm.com

[S31] C++：Hello World
来源：http://xnc.9152youxi.cn

#include <iostream>
来源：http://trs.chenlongwang.top

int main() { std::cout << "Hello\n"; }
来源：http://qes.haohaochexian.top

[S32] C++：字符串
来源：http://hnz.zhiwuduotai.top

std::string s = "hi";  s += "!";
来源：http://rrv.fktsv.cn

[S33] C++：vector 增删
来源：http://gbu.zdbjq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ptd.c1oappe.top

[S34] C++：遍历 vector
来源：http://ued.redwolf501.top

for (auto &x : v) { std::cout << x; }
来源：http://dfx.cheryme.top


<!-- 参考信息 -->