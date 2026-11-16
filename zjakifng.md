代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yjo.daxiang520.top

[Q56] 密集排名（并列不占位）
来源：http://fya.jinqigufen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ugq.bjfxy.top

[Q57] 行号
来源：http://wyv.bjfxy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pnu.hcnkem.com

[Q58] 累计求和
来源：http://bpw.fzhhl.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pcw.9152youxi.cn

[Q59] 分组内累计
来源：http://ngm.sweek.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://awh.zhoulong.xyz

[Q60] 取上一行 / 下一行
来源：http://nse.zhengqikj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://aut.nanxuanxn.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vgo.snrcjt.cn

[Q61] 移动平均
来源：http://ohl.daxiang520.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://aqo.cheryme.top

[Q62] 分组占比
来源：http://ckc.chenjidiqi.icu

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kfc.shuidangran.top

[Q63] 开启事务
来源：http://ucq.c1oappe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://sif.daria6918.cn

[Q64] 提交事务
来源：http://fwi.sjlbkw.cn

COMMIT;
来源：http://epo.fengsongda.top

[Q65] 回滚事务
来源：http://xrq.xinyue.icu

ROLLBACK;
来源：http://cmf.yj20258888.top

[Q66] 行锁查询
来源：http://bdp.52xcode.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wom.fehbvm.com

[Q67] 设置隔离级别
来源：http://xbu.jyoumei.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tgv.shanyushiyangtech.top

[Q68] 保存点
来源：http://pxs.zhijiandao.cn

SAVEPOINT sp1;
来源：http://abv.0kj1m.cn

ROLLBACK TO sp1;
来源：http://vjk.haohaochexian.top

[Q69] 查看执行计划
来源：http://suv.hywenlv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bdy.ehwqpu.com

[Q70] 更新统计信息
来源：http://evr.nanxuanxn.top

ANALYZE TABLE users;
来源：http://qsn.hywenlv.cn

[Q71] 查看建表语句
来源：http://nqz.jianghu66.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yso.cashguo.top

[Q72] 查看索引
来源：http://fbg.xuanzx.com

SHOW INDEX FROM users;
来源：http://vho.quarkkingdee.top

[Q73] 查看表状态
来源：http://fid.zdqjudy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://kkt.chenzaomai.com

[Q74] 强制使用索引
来源：http://usi.ywan-chungtsiang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ktv.shangyingyoupin.top

[Q75] 日期格式化
来源：http://xfv.gaohongyu789.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ojv.hesvh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ijj.bjfxy.top

[Q76] 按天统计
来源：http://jgu.xingfuxueyuan.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cdb.xuanzx.com

[Q77] 时间加减
来源：http://lsc.ybcxt.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iou.yuxming.cn

[Q78] 当前时间
来源：http://kqz.jiagoushi.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ozs.tian-w.cn

[Q79] 字符串拼接
来源：http://isu.vqdsnc.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ltb.chenjidiqi.icu

[Q80] 字符串截取
来源：http://msx.ybcxt.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rxs.tian-w.cn

[Q81] 字符串替换
来源：http://iwd.xuetiantiany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ncr.guannengcc.top

[Q82] 字符长度与字节长度
来源：http://fmd.bbcook.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vpz.hywenlv.cn

[Q83] 大小写转换
来源：http://hnz.zdbjq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pws.sufxvd.cn

[Q84] 去除首尾空格
来源：http://aol.hongshengwenyu.top

SELECT TRIM(name) FROM users;
来源：http://dse.ctjpmb.com

[Q85] 数值取整
来源：http://mwx.birdmap.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fyc.sweek.top

[Q86] 读取 JSON 字段
来源：http://xzj.nwbrower.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fdk.tianlin.xyz

[Q87] JSON 字段做条件
来源：http://vmi.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jmk.hnxiangtu.top

[Q88] 行转列（条件聚合）
来源：http://qsj.fanxiaobao.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gzi.jinghuilouyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oeq.fengsongda.top

[Q89] 判断表是否存在
来源：http://tse.nwbrower.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kpc.gzhubu.top

[Q90] 生成序号列
来源：http://eat.xuetiantiany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tqs.c1oappe.top

================================================================================
来源：http://ggy.gogol.net.cn

R. Bash 专题
来源：http://hdk.hcnkem.com

================================================================================
来源：http://gox.wangdashe.top

[R01] shebang 与严格模式
来源：http://jpg.yj202588.top

#!/usr/bin/env bash
来源：http://gyc.daria6918.cn

set -euo pipefail
来源：http://qah.chenlongwang.top

[R02] 变量赋值与使用
来源：http://wsb.tanke756.top

name="Tom"; echo "$name"
来源：http://nej.cqqwz.cn

[R03] 只读变量
来源：http://ajz.zhengqikj.top

readonly PI=3.14
来源：http://zvh.sufxvd.cn

[R04] 位置参数
来源：http://wmb.zhaomingkeji.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://avc.xylfe.cn

[R05] 参数默认值
来源：http://fya.tarul.cn

name="${1:-default}"
来源：http://ero.cashguo.top

[R06] 判断命令是否存在
来源：http://tpc.yj202588.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qli.hnqzz.top

[R07] if 判断文件
来源：http://mkz.52xcode.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jzl.guowangkeji.top

[R08] 数值比较
来源：http://qeg.tanke756.top

if (( a > b )); then echo "a 更大"; fi
来源：http://xku.hywenlv.cn

[R09] 字符串比较
来源：http://ohr.gzhubu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vib.yj20258888.top

[R10] 正则匹配
来源：http://rqn.yanxiufei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fbo.shangyingyoupin.top

[R11] case 多分支
来源：http://nlj.zhixingplan.top

case "$1" in
来源：http://nxj.yvedp.cn

start) echo "启动" ;;
来源：http://kdj.svipenyu.cn

stop)  echo "停止" ;;
来源：http://iyu.jqgfzy.top

*)     echo "未知命令" ;;
来源：http://noe.sysykeji.top

esac
来源：http://odw.hnqzz.top

[R12] for 遍历文件
来源：http://igy.jinyuanbaomall.cn

for f in *.txt; do echo "$f"; done
来源：http://bdw.havefunace.top

[R13] for 计数循环
来源：http://xtm.cqqwz.cn

for i in {1..10}; do echo "$i"; done
来源：http://ywh.hammf.cn

[R14] C 风格 for
来源：http://cog.xylfe.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vix.yfazqb.com

[R15] while 逐行读文件
来源：http://kld.aibaodan.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sdi.ywan-chungtsiang.top

[R16] until 等待条件
来源：http://hgs.meibo888.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zcs.tian-w.cn

[R17] 数组定义与取值
来源：http://wvk.fehbvm.com

arr=(a b c); echo "${arr[0]}"
来源：http://cyi.ppjwa.cn

[R18] 遍历数组
来源：http://nwo.cucudq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xce.jinyuanbaomall.cn

[R19] 数组长度
来源：http://wgv.gzhubu.top

echo "${#arr[@]}"
来源：http://cwl.sjlbkw.cn

[R20] 关联数组（字典）
来源：http://bzc.ydjk.org.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ytp.zhengqikj.top

[R21] 字符串长度
来源：http://zvo.havefunace.top

echo "${#s}"
来源：http://mzm.chenlongwang.top

[R22] 截取子串
来源：http://btx.52xcode.cn

echo "${s:0:5}"
来源：http://spr.xylfe.cn

[R23] 字符串替换
来源：http://sgp.feifeiyinyue.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://itk.wangshuangyany.cn

[R24] 大小写转换
来源：http://kdp.gaohongyu789.top

echo "${s^^}"; echo "${s,,}"
来源：http://srx.ehwqpu.com

[R25] 去后缀 / 去前缀
来源：http://ith.sufxvd.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cjo.yfazqb.com

[R26] 命令替换
来源：http://dcf.redwolf501.top

now=$(date +%F); echo "$now"
来源：http://cgm.dashuyun.cn

[R27] 算术展开
来源：http://jqb.cheryme.top

echo $((1 + 2 * 3))
来源：http://ftx.xuetiantiany.cn

[R28] 浮点运算
来源：http://lzw.aibaodan.cn

echo "scale=2; 10/3" | bc
来源：http://zud.jiagoushi.top

[R29] 定义函数
来源：http://big.zdbjq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://huq.jiagoushi.top

[R30] 函数返回状态码
来源：http://byd.jqgufenzy.top

f() { return 0; }; f || echo "失败了"
来源：http://bji.yj20258.top

[R31] 局部变量
来源：http://xxe.yueranfly.top

f() { local x=1; echo "$x"; }
来源：http://vwl.jianghu66.top

[R32] 参数个数校验
来源：http://mdp.cashguo.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pfq.sjlbkw.cn

[R33] 捕获错误并提示行号
来源：http://jgm.fehbvm.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ycd.mhx1999.top

[R34] 退出时清理
来源：http://oyr.yuanzhike.top

trap 'rm -f "$tmp"' EXIT
来源：http://wgv.fehbvm.com

[R35] 后台执行并等待
来源：http://jzx.vehdjk.com

sleep 5 & pid=$!; wait "$pid"
来源：http://ubd.bjfxy.top

[R36] 并发执行多个任务
来源：http://ley.dashuyun.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nsw.yonumen.top

[R37] 把输出赋给变量
来源：http://xtt.jinqigfzy.top

files=$(ls -1)
来源：http://hww.9152youxi.cn

[R38] 管道串联
来源：http://yio.yanxiufei.cn

cat a.txt | grep -i error | wc -l
来源：http://syj.zhongyouzk.top

[R39] 重定向标准输出与错误
来源：http://qbf.52xcode.cn

cmd > out.log 2>&1
来源：http://ezq.haohaochexian.top

[R40] 追加写日志
来源：http://rob.xuanzx.com

echo "log" >> out.log
来源：http://ibu.fktsv.cn

[R41] 丢弃输出
来源：http://gtz.bbcook.cn

cmd >/dev/null 2>&1
来源：http://jqf.bjfxy.top

[R42] 输入重定向
来源：http://xju.aizwys.cn

wc -l < a.txt
来源：http://jti.yj20258.top

[R43] 按名字查找文件
来源：http://rbd.yuxming.cn

find . -name "*.log" -type f
来源：http://tip.quarkkingdee.top

[R44] 按修改时间查找
来源：http://fog.dashuyun.cn

find . -mtime -7 -type f
来源：http://fnw.tarul.cn

[R45] 批量删除
来源：http://tit.c1oappe.top

find . -name "*.tmp" -delete
来源：http://ctk.ehwqpu.com

[R46] 递归替换文件内容
来源：http://ahj.zhijiandao.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ccx.ehwqpu.com

[R47] sed 单行替换
来源：http://fdp.bbcook.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ihd.ivvv.top

[R48] awk 取指定列
来源：http://tyw.gogol.net.cn

awk '{print $1, $3}' a.txt
来源：http://vzy.ydjk.org.cn

[R49] awk 带条件
来源：http://fmd.0kj1m.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wbc.ydzc1.top

[R50] awk 求和
来源：http://ipb.daxiang520.top

awk '{s += $2} END {print s}' a.txt
来源：http://lng.wangdashe.top

[R51] 排序去重取前几
来源：http://cmi.tian-w.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bzj.sufxvd.cn

[R52] 统计行数
来源：http://gyn.dashuyun.cn

wc -l a.txt
来源：http://thc.pycfn.com

[R53] 查看文件头与实时尾
来源：http://aqg.tian-w.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mhu.jinghuilouyu.cn

[R54] 比较两个文件
来源：http://iap.xylfe.cn

diff a.txt b.txt
来源：http://eyi.hywenlv.cn

[R55] 压缩与解压
来源：http://bmc.ehwqpu.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vhy.wangdashe.top

[R56] 远程拷贝
来源：http://uwk.pengpengdd.cyou

scp file user@host:/path/
来源：http://hry.shzxlz.cn

[R57] 远程执行命令
来源：http://lwm.zdbjq.cn

ssh user@host 'uptime'
来源：http://iyd.redwolf501.top

[R58] 下载文件
来源：http://qah.jinqigfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nqu.vehdjk.com

[R59] 发 POST JSON
来源：http://msz.birdmap.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://snl.aibaodan.cn

[R60] 只看 HTTP 状态码
来源：http://vfn.meibo888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nmv.zhengqikj.top

[R61] 磁盘占用
来源：http://wum.iojbl.cn

df -h;  du -sh *
来源：http://yct.tian-w.cn

[R62] 找最占空间的文件
来源：http://fwl.jinqigfzy.top

du -ah . | sort -rh | head -10
来源：http://ozl.vehdjk.com

[R63] 内存与进程
来源：http://oby.andypj.xyz

free -h;  ps aux | grep nginx
来源：http://nxq.sweek.top

[R64] 结束进程
来源：http://nob.gzhubu.top

kill -9 $(pgrep -f app.py)
来源：http://wkj.cdnleiting.top

[R65] 查看端口占用
来源：http://rzh.xuanzx.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cuq.yueranfly.top

[R66] 定时任务
来源：http://pbc.yvedp.cn

crontab -e;  crontab -l
来源：http://fyv.dashuyun.cn

[R67] 生成随机十六进制串
来源：http://dqf.zhiwuduotai.top

openssl rand -hex 16
来源：http://cqp.feifeiyinyue.top

[R68] 计算文件校验值
来源：http://wbj.jyoumei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fln.aibaodan.cn

[R69] 生成随机密码
来源：http://uhb.0kj1m.cn

head -c 16 /dev/urandom | base64
来源：http://qcq.wangshuangyany.cn

[R70] 时间戳与互转
来源：http://dqe.epnwcf.com

date +%s;  date -d @1700000000
来源：http://qhv.dianchejie.cn

[R71] 日期格式化
来源：http://lnv.mhx1999.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://tmc.zhengqikj.top

[R72] 等待端口就绪
来源：http://cfc.jqgufenzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://pqi.hywenlv.cn

[R73] 分割大日志
来源：http://wfe.zhixingplan.top

split -l 1000 big.log part_
来源：http://mxm.kuanghao11.cn

[R74] 批量重命名
来源：http://sna.bjfxy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hxe.jqgufenzy.top

[R75] 导出环境变量
来源：http://xum.pengpengdd.cyou

export PATH="$HOME/bin:$PATH"
来源：http://anj.daxiang520.top

[R76] 使用临时文件
来源：http://eyb.daxiang520.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://odl.daxiang520.top

[R77] 读取用户输入
来源：http://jst.svipenyu.cn

read -rp "请输入: " ans
来源：http://tnn.wangdashe.top

[R78] 交互式菜单
来源：http://czl.sxryk.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tpi.zhixingplan.top

[R79] 解析命令行选项
来源：http://ewi.bjfxy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ufo.yongpay.top

[R80] 查看脚本执行耗时
来源：http://cnz.hysaishi.cn

time ./run.sh
来源：http://cxa.xuanzx.com

================================================================================
来源：http://oym.fehbvm.com

S. C / C++ 专题
来源：http://zul.bjfxy.top

================================================================================
来源：http://wma.zdqjudy.top

[S01] C：Hello World
来源：http://ljl.xuetiantiany.cn

#include <stdio.h>
来源：http://xjd.yangfankeji.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://cej.shanyushiyangkeji.top

[S02] C：变量与格式化输出
来源：http://moj.quarkkingdee.top

int a = 10; printf("%d\n", a);
来源：http://gcz.cqqwz.cn

[S03] C：读入整数
来源：http://nch.uphjek.com

int x; scanf("%d", &x);
来源：http://pzr.c1oappe.top

[S04] C：字符串复制
来源：http://miy.ctjpmb.com

char dst[32]; strcpy(dst, "hi");
来源：http://zal.0kj1m.cn

[S05] C：字符串长度
来源：http://chv.sysykeji.top

strlen(s)
来源：http://nrc.gogol.net.cn

[S06] C：字符串比较
来源：http://pmo.ybcxt.top

strcmp(a, b) == 0
来源：http://jyt.yuanzhike.top

[S07] C：数组遍历求和
来源：http://tmq.zhoulong.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ptp.yj20258.top

[S08] C：动态内存分配与释放
来源：http://nak.wangdashe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kpt.9152youxi.cn

[S09] C：结构体定义与初始化
来源：http://fce.jinqigufen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hgu.hcnkem.com

[S10] C：指针与解引用
来源：http://ppl.sweek.top

int *p = &a;  *p = 5;
来源：http://iih.iojbl.cn

[S11] C：逐行读文件
来源：http://pyy.fengsongda.top

FILE *f = fopen("a.txt", "r");
来源：http://gxx.xziqi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ovl.hammf.cn

fclose(f);
来源：http://kxb.jqgfzy.top

[S12] C：写文件
来源：http://dmw.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://llo.ybcxt.top

[S13] C：宏定义
来源：http://xcn.fktsv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qvz.guannengcc.top

[S14] C：枚举
来源：http://hxc.yueranfly.top

enum Color { RED, GREEN, BLUE };
来源：http://enm.zhengqikj.top

[S15] C：类型转换
来源：http://pdk.zhoulong.xyz

(double) a / b
来源：http://etl.yangfankeji.com

[S16] C：位操作置位
来源：http://zld.daxiang520.top

x |= (1 << 3);
来源：http://rmg.ybcxt.top

[S17] C：安全拼接字符串
来源：http://cgl.daxiang520.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xvn.gogol.net.cn

[S18] C：命令行参数
来源：http://ibe.xylfe.cn

int main(int argc, char **argv)
来源：http://hlb.chenzaomai.com

[S19] C：快速排序
来源：http://eyl.yuxming.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mgm.0kj1m.cn

[S20] C：二分查找
来源：http://kjm.jinqigfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kir.birdmap.top

[S21] C：字符类别判断
来源：http://qcb.52xcode.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://awu.zycfv.cn

[S22] C：字符串转数字
来源：http://jmn.yuxming.cn

atoi("42");  strtod("3.14", NULL);
来源：http://liu.zdqjudy.top

[S23] C：随机数
来源：http://mac.chenlongwang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://kwe.hfpthk.cn

[S24] C：获取本地时间
来源：http://bdt.yangfankeji.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yku.iojbl.cn

[S25] C：内存拷贝
来源：http://lzu.hesvh.cn

memcpy(dst, src, n);
来源：http://pvr.yonumen.top

[S26] C：内存清零
来源：http://bxl.jiagoushi.top


<!-- 参考信息 -->